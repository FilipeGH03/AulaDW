<template>
    <div>
        <h1>Está é a descrição da pessoa:</h1>
        <p>O nome dela é: {{ nome }}</p>
        <p>Ela é profissional em: {{ profissao }}</p>
        <info :email="email" :estouTrabalhando= false></info>
        <info></info>
        <info></info>
        <Form></Form>
    </div>
</template>

<script>
    import info from './info.vue';
    import Form from './Form.vue';

    export default {
        name: "Pessoa",
        components: {
            info,
            Form
        },
        data() {
            return {
                nome: "tiringa",
                profissao: "tiringueiro",
                email: "aaaaaaaaaa@zzazzzzz",
            }
        }
    }


</script>