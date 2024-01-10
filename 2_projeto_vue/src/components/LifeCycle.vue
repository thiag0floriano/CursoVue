<template>
    <h1>Meu nome é: {{ nome }}</h1>
</template>

<script>
export default {
    nome: 'LifeCycle',
    data(){
        return {
            nome: 'Ainda não sei'
        }
    },
    created(){
        setTimeout(() => {
            this.nome = 'Thiago'     
        }, 1000);
    },
    mounted(){
        setTimeout(() => {
            this.nome = 'Sei lá...'     
        }, 2000);
    }
}

</script>