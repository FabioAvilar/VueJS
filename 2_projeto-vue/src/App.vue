<template>
  <div>
    <Header />
    <primeiro-componente />
    <p class="paragrafo-pai">O dado de app é: {{testando}}</p>
    <LifeCycle />
    <pessoa />
  </div>
</template>

<script>
  import PrimeiroComponente from './components/PrimeiroComponente.vue';
  import lifeCycle from './components/lifeCycle.vue';
  import LifeCycle from './components/lifeCycle.vue';
  import Pessoa from './components/pessoa.vue';
  import Header from './components/header.vue';

  export default {
    name: 'App',
    components: {
    PrimeiroComponente,
    lifeCycle,
    LifeCycle,
    Pessoa,
    Header
},
data() {
  return {
    testando: "Teste"
  }
}
  }
</script>

<style>
  body {
    background-color: #333;
    color: #fff;
  }

  a {
    color: red;
  }

  .teste {
    background-color: #000;
  }
</style>