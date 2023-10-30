<template>
    <!-- <Header></Header> -->
    <NavBar></NavBar>
    <RouterView></RouterView>
  <h1 class="paragrafo-pai">Aula DW </h1>
  <primeiroComponente></primeiroComponente>
  <p>Esse {{ name }}</p>
  <p>Vc? {{ teste }}</p>
  <pictures></pictures>
  <LifeCycle></LifeCycle>
  <Pessoa></Pessoa>
  <Form></Form>
</template>

<script>

import primeiroComponente from './components/primeiroComponente.vue';
import LifeCycle from './components/LifeCycle.vue';
import Pessoa from './components/Pessoa.vue';
import pictures from './components/pictures.vue';
// import Header from './components/Header.vue';
import NavBar from './components/NavBar.vue';
import { RouterLink } from 'vue-router';


export default {
  name: "App",
  components: {
    primeiroComponente,
    LifeCycle,
    Pessoa,
    pictures,
    // Header,
    NavBar,
    RouterLink
},


data(){
  return{
  name: "new",
  teste: "Fala calabreso"
}
}


}

</script>

<style>


  body {
    color: black;
    font-family: Inter, -apple-system, BlinkMacSystemFont, 'Segoe UI', Roboto, Oxygen, Ubuntu,
    Cantarell, 'Fira Sans', 'Droid Sans', 'Helvetica Neue', sans-serif;
  }

  .teste {
    color: blue;
  }


</style>