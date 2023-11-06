<template>
    <p>O status de tudo no começo é um {{ name }}</p>
    <MultiplosEventos></MultiplosEventos>
</template>

<script>

import MultiplosEventos from './MultiplosEventos.vue';

export default {

    name: "primeiroComponente",

    components:{
        MultiplosEventos
    },

    data(){
        return {
        name: "inicio positivo."
    }
    }

}

</script>