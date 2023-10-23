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
        <p v-show="mostrarEmail">Fala com os guri ai {{email}}</p>
        <p class="teste">Para acessar meu curriculo click aqui, <a v-bind:href="link">Aqui songo mongo</a> </p>

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