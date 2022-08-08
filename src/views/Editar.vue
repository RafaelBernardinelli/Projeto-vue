<template>
<div class=" main-container">
    <div class="rotas">
    <router-link class="links" to="/">Home </router-link>>
    <router-link class="links" to="/Editar">Editar Produto</router-link>
    </div>
    <div>
        <h1>Editar Produtos</h1>
    </div>
    <Form />
</div>
</template>

<script>
import Form from '../components/Form.vue'
export default {
  components: { Form },
    name: "Editar"
}


</script>

<style>

</style>