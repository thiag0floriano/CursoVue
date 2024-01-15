<template>
    <h1>Olá Vue!</h1>
    <p>Sera que deu certo? {{ resposta }} é agora ? {{ fala }}</p>
    <MultiplosEventos />
</template>

<script>
    import MultiplosEventos from './MultiplosEventos.vue';
    export default {
        name: 'ComponenteCerto',
        components:{
            MultiplosEventos
        },
        data() {
            return {
                resposta: "deu Certo sim.",
                fala: "Então vamos que, vamos!"
            }
        }
    }
</script>