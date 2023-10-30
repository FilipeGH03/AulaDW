<template>
    <div>
        <p>Ela utiliza as seguintes tecnologias:</p>
        <p v-if="trabalhar">Não quero trabalhar</p>
        <p v-else >Não quero faze nada</p>
        <ul>
            <li v-for="tecnologia in listatecnologia" v-bind:key="index">{{ tecnologia }}</li>

        </ul>
        <p>Utilizo seguintes ferramentas</p>
        <ul>
            <li v-for="tecnologia in listaferramenta" v-bind:key="tecnologia.id">{{ tecnologia.ferramenta }}</li>
        </ul>
        <div>
            <button @click="showemail">Email mostrar</button>
        </div>
        <p v-show="mostrarEmail">Fala com os guri ai {{email}}</p>
        <p class="teste">Para acessar meu curriculo click aqui, <a v-bind:href="link">Clique aqui</a> </p>

    </div>
</template>

<script>

    export default {
        name: "Info",
        
        data() {
            return {
                trabalhar: false,
                mostrarEmail: false,
                email: "tiringa.terra@gmail.com",
                link: 'https://www.chess.com',
                listatecnologia: ["JavaScript", "Vue", "HTML"],
                listaferramenta: [
                    {id:1, ferramenta: 'Chess'},
                    {id:2, ferramenta: 'Class'},
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