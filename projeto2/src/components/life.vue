<template>
    <p>{{ name }}</p>
</template>

<script>
export default{
    name:'life',
    data(){
        return{
            name:"testar"
        }
    },
    created(){
        setTimeout(() =>{
            this.name = "nome"
        },1000)
    },
    mounted(){
        setTimeout(() =>{
            this.name= "aa"
        },2000)
    }
}
</script>