<template>
    <div>
        <p>Ela utiliza as seguintes tecnologias:</p>
        <p v-if="trabalhar">Não quero trabalhar</p>
        <p v-else >Não quero faze nada</p>
        <ul>
            <li>JavaScript</li>
            <li>Vue</li>
            <li>HTML</li>
        </ul>
        <p v-show="mostrarEmail">Fala cos guri ai{{email}}</p>
        <p>Para acessar meu curriculo click aqui, <a v-bind:href="link">Aqui songo mongo</a> </p>
    </div>
</template>

<script>
    export default {
        name: "Info",
        data() {
            return {
                trabalhar: false,
                mostrarEmail: true,
                email: "iouiysufdyghiajoskpd@gmail.com",
                link: 'https://www.chess.com'
            }
        }
    }
</script>