<template>
    <h2>Testando minha lista de array</h2>
    
    <ul>
        <li v-for="(listaTeste, index) in lista1" v-bind:key="index"> {{ listaTeste }} </li>
    </ul>

</template>

<script>
    export default{
        nome: 'ListaDeArray',
        components: {

        },
        data(){
            return{
                lista1: ['Item 1','Item 2','Item 3']
            }
        }
    }
</script>