<template>
    <Reutilizacao />
    <h1>Olá Vue!</h1>
    <Reutilizacao />
    <p>Sera que deu certo? {{ resposta }} é agora ? {{ fala }}</p>
    <MultiplosEventos />
    <Reutilizacao />
    <Reutilizacao />
    <Reutilizacao />
    <Reutilizacao />
    <Reutilizacao />
    <Reutilizacao />
</template>

<script>
    import Reutilizacao from './Reutilizacao.vue';
    import MultiplosEventos from './MultiplosEventos.vue';
    export default {
        name: 'ComponenteCerto',
        components:{
            MultiplosEventos,
            Reutilizacao
        },
        data() {
            return {
                resposta: "deu Certo sim.",
                fala: "Então vamos que, vamos!"
            }
        }
    }
</script>