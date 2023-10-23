<template>
    <div>
        <p>Ela utiliza as seguintes tecnologias:</p>
        <p v-if="trabalhar">Não quero trabalhar</p>
        <p v-else >Não quero faze nada</p>
        <ul>
            <li>Lábia</li>
            <li>Xadrez</li>
            <li>Banheiro</li>
        </ul>

        <div>
            <button @click="showemail">Email mostrar</button>
        </div>
        <p v-show="mostrarEmail">Fala com os guri ai{{email}}</p>
        <p>Para acessar meu curriculo click aqui, <a v-bind:href="link">Aqui songo mongo</a> </p>
        <pictures></pictures>

    </div>
</template>

<script>

import pictures from './pictures.vue';
    export default {
        name: "Info",
        components: {
            pictures,
        },
        data() {
            return {
                trabalhar: false,
                mostrarEmail: false,
                email: "tiringa.terra@gmail.com",
                link: 'https://www.chess.com',
            }
        },
        methods:{
            showemail(){
                // console.log("TEste email")
                this.mostrarEmail = !this.mostrarEmail
            }
        }
    }
</script>