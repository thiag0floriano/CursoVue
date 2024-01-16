<template>
    <div>
        <button @click="primeiro(txt1, $event), segundo(txt2, $event), terceiro($event)">Ativar mútiplos eventos</button>
        <p>{{ multiplos_eventos }}</p>
    </div>
    
</template>

<script>
    export default {
        name: 'MultiplosEventos',
        data(){
            return {
                multiplos_eventos: "",
                txt1: "Primeiro evento!",
                txt2: "Segundo eventos!"
            }
        },
        methods:{
            primeiro(e){
                this.multiplos_eventos = this.txt1
            },
            segundo(e){
                setTimeout(() => this.multiplos_eventos = this.txt2, 500)
            },
            terceiro(e){
                setTimeout(() => this.multiplos_eventos = "", 1500)
            }
        }
    }
</script>

<style scoped>
    div{
        margin: 100px;
    }

</style>