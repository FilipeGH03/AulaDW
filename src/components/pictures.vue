<template>
    <img :src="avatar" alt="descricao">
    <MudarImagem @mudar-imagem="trocarImagem"></MudarImagem>
</template>


<script>
import MudarImagem from './MudarImagem.vue';
    export default {
        name: 'pictures',
        data(){
            return{
                avatar:'img/avatar.png',
                descricao: "avatar de cria"
            }
        },
        components:{
            MudarImagem
        },

        methods:{
            trocarImagem(){
            this.avatar = "img/avatar2.png"
        }, }}
</script>