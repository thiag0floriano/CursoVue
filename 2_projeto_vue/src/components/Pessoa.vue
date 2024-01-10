<template>
    <h2>Etaá é a descrição da passoa: </h2>
    <info />
</template>

<script>
    import info from './info.vue';
    export default {
        name: 'Pessoa',
        components: {
            info
        },
        data(){
            return {
                nome: 'Thiago'
            }
        }
    }
    
</script>