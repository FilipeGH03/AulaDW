<template>
  <h1>Vamooo funciono</h1>
  <primeiroComponente></primeiroComponente>
  <p>Esse {{ name }}</p>
  <p>Oureo {{ teste }}</p>
  <LifeCycle></LifeCycle>
  <Pessoa></Pessoa>
  <Form></Form>
</template>

<script>

import primeiroComponente from './components/primeiroComponente.vue';
import LifeCycle from './components/LifeCycle.vue';
import Pessoa from './components/Pessoa.vue';


export default {
  name: "App",
  components: {
    primeiroComponente,
    LifeCycle,
    Pessoa
},

data(){
  return{
  name: "Will",
  teste: "Oi"
}
}


}

</script>