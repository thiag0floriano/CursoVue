<template>
    <div>
        <h2>Testando minha lista com objeto</h2>
        <ul>
            <li v-for="objetoTeste in objeto1" :key="objetoTeste.id">
                {{ objetoTeste.item }}
            </li>
        </ul>
    </div>

</template>

<script>
    export default{
        nome: 'ListaDeObjeto',
        components: {

        },
        data(){
            return{
                objeto1: [
                    {id: 1, item: 'Item 1'},
                    {id: 2, item: 'Item 2'},
                    {id: 3, item: 'Item 3'}
                ]
            }
        }
    }
</script>