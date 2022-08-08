<template>
    <ul>
        <li v-for="Produtos in DescricaoDeProdutos" :key="Produtos.id">
        {{ Produtos.Descricao }}
        </li>
    </ul>
</template>

<script>
export default {
    name: "ProdutosHome",
    data() {
        return {
            DescricaoDeProdutos: [
                {id: 1, Descricao: "camera"},
                {id: 2, Descricao: "camera2"},
                {id: 3, Descricao: "camera3"},
            ]
        }
    }
}
</script>