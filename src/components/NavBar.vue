<template>
    <div id="nav">
        <router-link to="/">
        <img :src="logo" alt="alt" id="logo">
        </router-link>
        
    </div>
</template>
<script>
export default {
    name: "NavBar", 
    props: ["logo", "alt"]
}
</script>

<style scoped>

    #nav {
        background-color: #00264b;
        text-align: center;
    }
    #nav img {
        width: 16%;
        padding: 17px;
    }
</style>

