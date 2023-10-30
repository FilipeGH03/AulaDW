<template>
    <div>
        <ul>
            <li><a href="#">Home</a></li>
            <li><a href="#">saiba mais</a></li>
            <li><a href="#">Escola</a></li>
            <li><a href="#">faculdade</a></li>
        </ul>
    </div>
</template>

<script>


export default {

    name:"Header"
}
</script>


<style scoped> 


    ul {
        list-style: none;
        display: flex;
        justify-content: space-around;

    }

    a {
        color: rgb(60, 0, 255);
        text-decoration: none;
        font-size: 22px;
    }

</style>