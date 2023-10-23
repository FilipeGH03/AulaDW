<template>
    <div>
        <ul>
            <li><a href="#">Calabreso</a></li>
            <li><a href="#">CNPJoto</a></li>
            <li><a href="#">Arabio Saudito</a></li>
            <li><a href="">Ludmilo</a></li>
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