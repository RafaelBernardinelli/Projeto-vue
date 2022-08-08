<template>
    <div class="form">
     <form v-on:submit.prevent="postProduto">
      <div class="text">
        <label>Nome do produto:</label>
        <input
          type="text-t"
          v-model="nome"
          placeholder="Digite o nome do produto"
          required
        />
      </div>
      <div class="text">
        <label>Marca:</label>
        <input
          type="text"
          v-model="marca"
          placeholder="Digite a marca do produto"
          required
        />
      </div>
      <div class="textD">
        <label>Valor:</label>
        <input type="number" v-model="valor" placeholder="R$00,00" required />
      </div>
      <div class="textD">
        <label>Cor</label>
        <select v-model="cor" required>
          <option disabled value="">Selecione a cor</option>
          <option>Branco</option>
          <option>Cinza</option>
          <option>Preto</option>
        </select>
        
      </div>
      <div class="textD">
        <label>Data de Cadastro:</label>
        <input
          type="date"
          required
        />
      </div>
      <div class="botao">
        <div>
            <button class="file">
          <input class="btn" @change="handleImage" type="file" required />
          </button>
        </div>
        <div v-if="imagem != null">
          <img :src="imagem" />
        </div>
      </div>
      <div class="text">
        <button class="submit-btn" type="submit">
          ADICIONAR PRODUTO
          <Message :msg="msg" v-show="msg" />
        </button>
      </div>
    </form>
    </div>
</template>

<script>
export default {
    name: "Form",
}
</script>

<style scoped>
.form {
    margin-top: 50px;
}
.text{
    margin-top: 10px;
    flex-direction: column;
    display: flex;
}
.textD{
    margin-top: 10px;
    flex-direction: column;
    display: flex;
    width: 30%;
}
input,
select {
  height: 45px;
  font-size: 20px;
  padding-left: 5px;
  border-radius: 5px;
}
.submit-btn {
    width: 30%;
    height: 38px;
    background-color: #00264b;
    border: none;
    border-radius: 5px;
    color: white;
    margin-top: 20px;
}
.btn {
    display: none;
}
.file {
}
.botao {
    width: 150px;
    margin-top: 25px ;
    height: 140px;
    border: 1px dashed;
    border-radius: 5px;
}

</style>