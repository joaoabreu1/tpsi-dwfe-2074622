<template>
    <h1> {{numero}}</h1>
    <button @click="somar()">clica-me!</button>
</template>

<script>
export default{
    name: 'Nova',
    data(){
        return{
            titulo: 'TPSI',
            numero: 0
        }
        },
    methods:{
        somar(){ //função para somar 1 ao numero
            this.numero++
            }
        }
    }
</script>