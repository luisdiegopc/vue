<template>
  <!-- Importação OK 
  <div id="app">
    <h1> Meu Teste </h1>
    <ExBootstrap />
  </div> -->

  <div id="app">
     
    <ExAPI />
  </div>


</template>

<script>
// Importe o componente  *******--------

// import ExBootstrap from './components/ExBootstrap.vue';
 
import ExAPI from './components/ExAPI.vue';
 
/* export default {
    name: 'App',
    // Registre o componente
    components: {
      ExBootstrap,
  },
}; */

export default {
    name: 'App',
    // Registre o componente
  components: {
      ExAPI,
  },
};

</script>