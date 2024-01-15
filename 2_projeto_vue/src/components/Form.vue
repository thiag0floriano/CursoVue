<template>
    <form action="" @Submit="enviarFormulario($event)">
        <h1>Meu Formulario</h1>
        <div>
            <!-- <InputText /> -->
            <input type="text" v-model="nome">
        </div>
        <div>
            <!-- <InputText /> -->
            <input type="text" v-model="email">
        </div>
        <div>
            <Submit />
        </div> 
    </form>
</template>

<script>
    import InputText from'./form/InputText.vue';
    import Submit from './form/Submit.vue';
    export default {
        name: 'Form',
        components: {
            InputText,
            Submit
        },
        data() {
            return {
                nome: '',
                email: ''
            }
        },
        methods: {
            enviarFormulario(e){

                e.preventDefault();

                const nome = this.nome;
                const email = this.email;

                console.log("Formulario Enviado!");
                console.log("O nome é: "+ nome);
                console.log("O email é: "+ email);
            }
            
        }    
    }
</script>