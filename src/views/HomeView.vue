<template>
  <div class="main-container">
    <div class="cima">
      <div class="titulo"><h1>Produtos</h1></div>
      
      <div class="button">
      <button class="btn" ><svg class="icone" width="15" height="15" viewBox="0 0 32 32" fill="none" xmlns="http://www.w3.org/2000/svg">
      <path d="M16.0016 32C7.16818 31.9903 0.00970076 24.8325 0 16V15.68C0.175908 6.88727 7.41608 -0.115241 16.2107 0.00143715C25.0053 0.118115 32.0571 7.31024 31.9997 16.1046C31.9422 24.8989 24.797 31.9982 16.0016 32ZM8.0008 14.4V17.6H14.4014V24H17.6018V17.6H24.0024V14.4H17.6018V8.00002H14.4014V14.4H8.0008Z" fill="white"/>
      </svg>
      <router-link class="btn" to="/Adicionar"> Adicionar Produto</router-link>
      </button>
      </div>
    </div>
    <ProdutosHome />
    <icons />
  </div>
</template>

<script>
import icons from '@/components/icons.vue'
import ProdutosHome from '@/components/ProdutosHome.vue';
export default {
  components: {
    ProdutosHome,
    icons,
}
}

</script>
<style scoped>
.main-container {
    width: 1200px;
    /* alinhar o main ao centro */
    font-family: Raleway;

}
.btn {
  background-color:#0f4c81;
  text-decoration: none;
  color: white;
  height: 35px;
  width: 220px;
  border: none;
  border-radius: 5px;
  font-size: 20px;

}
.titulo {
  justify-content: space-between;
  display: flex;
}
.button {
  justify-content: space-between;
  display: flex;
}
.cima {
  display: flex;
  justify-content: space-between;
  margin-top: 60px;
}
</style>