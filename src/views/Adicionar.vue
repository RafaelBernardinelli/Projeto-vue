<template>
<div class=" main-container">
  <div class="rotas">
    <router-link class="links" to="/">Home </router-link>>
    <router-link class="links" to="/Adicionar">Adicionar Produto</router-link>
  </div>
    <div>
      <h1>Adicionar Produto</h1> 
      <Form />
    </div>
    
</div>
</template>

<script>
import Form from "../components/Form.vue"
export default {
    name: "Adicionar",
    components: {
      Form,
    },
}
</script>

<style>

</style>