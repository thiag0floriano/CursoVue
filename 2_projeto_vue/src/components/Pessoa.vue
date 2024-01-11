<template>
    <h2>Etaá é a descrição da passoa: </h2>
    <Info />
    <Form />
</template>

<script>
    import Info from './Info.vue';
    import Form from './Form.vue';
    export default {
        name: 'Pessoa',
        components: {
            Info,
            Form
        },
        data(){
            return {
                nome: 'Thiago'
            }
        }
    }
    
</script>