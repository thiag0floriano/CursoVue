<template>
    <h1>Olá Vue!</h1>
    <p>Sera que deu certo? {{ resposta }} é agora ? {{ fala }}</p>
</template>

<script>
    
    export default {
        name: 'ComponenteCerto',
        data() {
            return {
                resposta: "deu Certo sim.",
                fala: "Então vamos que, vamos!"
            }
        }
    }
</script>