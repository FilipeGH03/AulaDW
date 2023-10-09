<template>
    <h1>{{ name }}</h1>
</template>

<script>

export default  {
    name:"Life Cycle",
    data(){
        return{
            name: "Testar alguma coisa mt massa"
        }

    },

    created(){
        setTimeout(() => {
            this.name = "Will mt massa"
        }, 1000)
        
    },
    mounted(){
        setTimeout(() => {
            this.name = "Ouro alfujem"
        },1000)
        
    }

}


</script>