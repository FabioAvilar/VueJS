<template>
  <div>
    <primeiro-componente />
    <p>O dado de app é: {{testando}}</p>
    <LifeCycle/>
  </div>
</template>

<script>
  import PrimeiroComponente from './components/PrimeiroComponente.vue';
  import lifeCycle from './components/lifeCycle.vue';
import LifeCycle from './components/lifeCycle.vue';

  export default {
    name: 'App',
    components: {
    PrimeiroComponente,
    lifeCycle,
    LifeCycle
},
data() {
  return {
    testando: "Teste"
  }
}
  }
</script>