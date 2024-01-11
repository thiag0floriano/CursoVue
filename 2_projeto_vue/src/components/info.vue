<template>
    <div>
        <p v-if="esta_trabalhando">Estou trabalhado no momento.</p>
        <p v-else>Estou em busca de novas oportunidades!</p>
        <p>Utilizo as seguintes tecnologias para back-end:</p>
        <ul v-for="technology in backend_technologies">
            <li>{{ technology }}</li>
        </ul>
        <div>
            <button @click="showEmail">{{ textoBotao }}</button>
        </div>
        <p v-show="mostrar_email">Mande ua mensagem para: {{ email }}</p>
        <p class="teste">Para acessa o meu portfólio <a v-bind:href="meu_link" target="_blank">basta clicar aqui</a></p>
        <Picture />
    </div>
</template>

<script>
    import Picture from './Picture.vue';
    export default {
        name: 'Info',
        components: {
            Picture
        },
        data(){
            return{
                esta_trabalhando: false,
                mostrar_email: false,
                email: 'thiago@oops.net.br',
                meu_link: 'https://google.com',
                textoBotao: "Mostrar e-mail",
                backend_technologies: ['','','']
            }
        },
        methods: {
            showEmail(){
                this.mostrar_email = !this.mostrar_email
                if(!this.mostrar_email){
                    this.textoBotao = "Mostra e-mail"
                }else{
                    this.textoBotao = "Esconder e-mail"
                }
            }
        }
    }
</script>