<template>
    <div>
        <h1>Está é a descrição da pessoa:</h1>
        <p>O nome dela é: {{ nome }}</p>
        <p>Ela é profissional em: {{ profissao }}</p>
        <infoVue></infoVue>
        <infoVue></infoVue>
        <infoVue></infoVue>
        <Form></Form>
    </div>
</template>

<script>
    import infoVue from './info.vue';
    import Form from './Form.vue';

    export default {
        name: "Pessoa",
        components: {
            infoVue,
            Form
        },
        data() {
            return {
                nome: "will",
                profissao: "stope"
            }
        }
    }


</script>