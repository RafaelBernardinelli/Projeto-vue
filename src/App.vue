<template>
<div>
  <NavBar :logo="logo_src" :alt="app_name" />
  <div>
  <router-view />
  </div>
</div>
</template>

<script>
import NavBar from './components/NavBar.vue';


export default {
  components: {
    NavBar,
},
  data() {
    return {
      logo_src: "img/logo.png",
      app_name: "VipTech"
    }
  }
}

</script>

<style>
  * {
    margin: 0;
    padding: 0;
    box-sizing: border-box;
    font-family: Raleway;
    
  }
 
  .main-container {
    width: 1050px;
    height: 100%;
    margin-left: 300px;
    margin-top: 30px;
  }
  .rotas {
    margin-bottom: 30px;
  }
  .links {
    text-decoration: none;
    color: #00264b;
  }
</style>
