<template>
  <div id="app">
    <h1> Meu Teste </h1>
    <ExBootstrap />
  </div>
</template>

<script>
// Importe o componente
 import ExBootstrap from './components/ExBootstrap.vue';
export default {
  name: 'App',
  // Registre o componente
  components: {
    ExBootstrap,
  },
};



</script>