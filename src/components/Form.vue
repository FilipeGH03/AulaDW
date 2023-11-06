<template>

    <form action="" @submit="enviarFormulario($event)">
        <div>
            <input type="text" v-model="name">
            <input type="text" v-model="email">
            <Submit></Submit>
        </div>
    </form>

</template>

<script>


import InputText from './Form/InputText.vue';
import Submit from './Form/Submit.vue';


    export default{
        name: 'Form',
        components:{
            InputText,
            Submit
        },

        data(){
            return {
                name: "",
                email: ""
            }
        },

        methods: {
            enviarFormulario(e){
                e.preventDefault();
                
                let name = this.name;
                let email = this.email;
                console.log("o nome é " + name + " o email é " + email)
                console.log("form enviado")
            }
        }
      };

    
</script>