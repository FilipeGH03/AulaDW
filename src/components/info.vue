<template>
    <div>
        <!-- <p>{{ compEmail }}</p> -->
        <p>Ela utiliza as seguintes tecnologias:</p>
        <p v-if="trabalhar">Funcionou o trabalaho:</p>
        <p v-else >Positivo aqui</p>
        <ul>
            <li v-for="tecnologia in listatecnologia" v-bind:key="index">{{ tecnologia }}</li>

        </ul>
        <p>Utilizando seguintes ferramentas</p>
        <ul>
            <li v-for="tecnologia in listaferramenta" v-bind:key="tecnologia.id">{{ tecnologia.ferramenta }}</li>
        </ul>
        <div>
            <button @click="showemail">Email mostrar</button>
        </div>
        <p v-show="mostrarEmail">Contato fala ai {{email}}</p>
        <p class="teste">Para acessar meu curriculo click aqui, <a v-bind:href="link">Clique aqui</a> </p>

    </div>
</template>

<script>

    export default {
        name: "Info",
        
        props: {
            email : String,
            estouTrabalhando : Boolean,
        },



        data() {
            return {
                trabalhar: false,
                mostrarEmail: false,
                // email: "aaaaaaaa_@gmail.com",
                link: 'https://www.google.com',
                listatecnologia: ["Riot", "HTML", "Steam"],
                listaferramenta: [
                    {id:1, ferramenta: 'Figma'},
                    {id:2, ferramenta: 'Chess'},
            ]
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


<style>
    .paragrafo-pai {
        color: blueviolet;
    }
</style>