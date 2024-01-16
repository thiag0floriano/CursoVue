<template>
    <div>
        <h2>Etá é a descrição da passoa: </h2>
        <Info :email = "email"/>
        <Form />
    </div>
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
                nome: 'Thiago',
                email: "thiago@oops.net.br"
            }
        }
    }
    
</script>