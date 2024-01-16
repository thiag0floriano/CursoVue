<template>
    <div>
        <img :src="avatar" :alt="descricao">
        <MudarImagem @mudar-imagem="trocarImagem" />
    </div>
</template>

<script>
import MudarImagem from './MudarImagem.vue';

export default{
    name: 'Picture',
    components: {
        MudarImagem
    },
    data() {
        return {
            avatar: "/img/avatar.png",
            descricao: "Imagen Avatar"
        };
    },
    components: { 
        MudarImagem 
    },
    methods: {
        trocarImagem() {
            console.log("Opa")
        }
    }
}
</script>