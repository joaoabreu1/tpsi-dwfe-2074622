<template>
   

    <div class="centro"> <!-- div para o centro -->
        <br><br>

        <input type="number"  @input="num1" v-model="num1">
        <p>+</p>
        <input type="number" @input="num2" v-model="num2">
        <br>
        <br>
        <button @click="total()">calcular!</button>
        <p>Resultado: {{resultado}}</p>
    </div>

     <div class="left">  <!-- div para a esquerda -->
        <h1>{{titulo}}</h1>
        <button @click="somar()">clica-me!</button>
        <h1> {{numero}}</h1>
    </div>
</template>

<script>

export default{
    name: 'Nova', //variáveis
        data(){
            return{
                titulo: 'TPSI',
                numero: 0,
                num1: 0,
                num2: 0,
                resultado: 0,
            }
        },
    methods:{
        somar(){ //função para somar 1 ao indicador
                this.numero++
            },

        total(){ //função para calcular o total
                this.resultado = parseInt(this.num1) + parseInt(this.num2);
            },
        },
}   

</script>

