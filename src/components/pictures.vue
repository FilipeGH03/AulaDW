<template>
    <img :src="avatar" alt="descricao">
</template>


<script>
    export default {
        name: 'pictures',
        data(){
            return{
                avatar:'img/avatar.png',
                descricao: "avatar de cria"
            }
        }
    }
</script>