<template>

    <div>
        <button @click="primeiro(txt1, $event), segundo(txt2 ,$event)" >Ativar eventos</button>
        <p>{{ multiplos_eventos }}</p>
    </div>

</template>


<script>
    export default {
        name: "MultiplosEventos",
        data(){
            return{
                multiplos_eventos: "",
                txt1 : "Primeiro evento",
                txt2 : "Segundo evento"
            }
        },

        methods:{
            primeiro(txt1, e){
                this.multiplos_eventos = txt1;
            },

            segundo(txt2, e) {
                setTimeout(() => this.multiplos_eventos = txt2, 2000) 
            }
        },

    }

    

    

</script>