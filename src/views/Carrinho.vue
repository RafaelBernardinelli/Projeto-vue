<template>
    <div class=" main-container">
        <div class="rotas">
            <router-link class="links" to="/">Home </router-link>>
            <router-link class="links" to="/Carrinho">Carrinho</router-link>
        </div>
        <div className="gridColumn">
            <div>
                <h1>Carrinho</h1>
            </div>
            <div className="Resumo">
                <h1>Resumo do Pedido</h1>
            </div>
        </div>
        <div className="gridColumn">
            <div className="grid1">
                <div>
                    <div className="grid2">
                        <div className="grid3">
                            <div>

                            </div>
                        </div>
                        <div className="grid4">
                            <div class="gride">
                                <h3>Modelo</h3>
                                <p>Marca</p>
                                <p>Cor: Branco</p>
                            </div>
                        </div>
                    </div>
                    <hr />
                    <div>
                        <div className="btnQtd">
                            <div class="div">
                                Quantidade:
                            </div>
                            <div class="btns">
                                <Button>
                                    <svg width="30" height="30" viewBox="0 0 32 33" fill="none"
                                        xmlns="http://www.w3.org/2000/svg">
                                        <path d="M9 18.5V15.5H23V18.5H9Z" fill="#353535" />
                                        <circle cx="16" cy="16.5" r="15.5" stroke="#353535" />
                                    </svg>
                                </Button>
                                <p className="contador">1</p>
                                <Button>
                                    <svg width="30" height="30" viewBox="0 0 32 32" fill="none"
                                        xmlns="http://www.w3.org/2000/svg">
                                        <path d="M17 17.5V23.5H15V17.5H9V15.5H15V9.5H17V15.5H23V17.5H17Z"
                                            fill="#353535" />
                                        <circle cx="16" cy="16" r="15.5" stroke="#353535" />
                                    </svg>
                                </Button>
                            </div>
                            <div class="total">
                            <p class="total">R$ 349,00</p>
                            </div>
                        </div>
                    </div>
                </div>
            </div>

        </div>
    </div>
</template>

<script>
export default {
    name: "Carrinho"
}

</script>

<style scoped>
.main-container {
    width: 1200px;
    height: 650px;
}

.contador {
    border: 1px solid gray;
    border-radius: 5px;
    margin: 2px;
    padding: 7px 15px 7px 15px;
}
.grid-Column {
    display: flex;
    justify-content: space-between;
}

.grid1 {
    margin-top: 20px;
    border-radius: 5px;
    display: flex;
    border: solid 1px #B2B2B2;
    height: 250px;
    width: 750px;
    flex-direction: column;
    padding: 25px;
}

.grid2 {
    height: 150px;
    width: 750px;
    display: flex;
}

.grid3 {
    width: 150px;
    height: 150px;
    display: flex;
    justify-content: center;
}

.grid4 {
    width: 600px;
    height: 150px;
    display: flex;
}

.btnQtd {
    font-weight: bold;
    font-size: 20px;
    height: 40px;
    width: 750px;
    display: flex;
    margin-top: 25px;
    align-items: center;
}

.pagamento {
    margin-top: 10px;
    height: 180px;
    border: solid 1px #039500;
    border-radius: 10px;
    text-align: center;
    color: #039500;
    font-size: 18px;
    font-weight: bold;
    width: 100%;
    height: inherit;
    position: relative;
    margin-top: 10px;
    overflow: visible;

}
.total {
    margin-right: 10px;
}

.pagar {
    background-color: #f5f5f5;
    margin-top: 20px;
    height: 290px;
    border-radius: 5px;
    padding: 10px 24px 0 24px;
    font-size: 20px;
    font-weight: bold;
}

.cedulas {
    font-size: 16px;
}

.cedulas p {
    line-height: 12px;

}

.pagamento h2 {
    font-weight: bold;
    font-size: 18px;
}

.valorTotal {
    display: flex;
    justify-content: space-between;
    line-height: 2px;
}

.divFrete {
    display: flex;
    justify-content: space-between;
    line-height: 2px;
    margin-bottom: 20px;
}

.divSubtotal {
    display: flex;
    justify-content: space-between;
    line-height: 2px;
}

.gride {
    padding-left: 15px;
    align-items: center;
    margin-top: 20px;
}

.div {
    width: 150px;
    text-align: center;
}

.btns {
    display: flex;
    width: 480px;
}
.btns {
   border: 1px solid transparent;
   background: transparent;
}
</style>