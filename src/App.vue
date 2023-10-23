<template>
    <Header></Header>
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
import Header from './components/Header.vue';


export default {
  name: "App",
  components: {
    primeiroComponente,
    LifeCycle,
    Pessoa,
    pictures,
    Header

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
    background-color: rgb(128, 206, 209);
    color: aliceblue;
    font-family: Inter, -apple-system, BlinkMacSystemFont, 'Segoe UI', Roboto, Oxygen, Ubuntu,
    Cantarell, 'Fira Sans', 'Droid Sans', 'Helvetica Neue', sans-serif;
  }

  .teste {
    color: blue;
  }


</style>