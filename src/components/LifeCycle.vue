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
            this.name = "legal né mt massa"
        }, 1000)
        this.lifeCycle()
        
    },
    mounted(){
        setTimeout(() => {
            this.name = "Aquele cara la"
        },1000)
        
    },

    methods: {
        lifeCycle(){
            console.log ("alguma coisa")
        }
    }

}


</script>