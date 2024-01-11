<template>
    <form action="">
        <h1>Meu Formulario</h1>
        <div>
            <InputText />
        </div>
        <div>
            <InputText />
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
        data(){
            return{

            }
        }
    }
</script>