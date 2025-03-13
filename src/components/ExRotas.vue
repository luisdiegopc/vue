<!-- Estrutura extraída do site: https://vuejs.org/guide/scaling-up/routing.html -->

<!-- SCRIPT -->
<script setup>
  // Importações do Vue
  import { ref, computed } from 'vue'

  // Páginas
import ExPagina1 from './ExPagina1.vue'
import ExPagina2 from './ExPagina2.vue'
import ExPaginaErro from './ExPaginaErro.vue'

  // Criar uma estrutura de rotas, contendo o caminho e o camponente
  const routes = {
    '/': ExPagina1,
    '/Expagina2': ExPagina2,
    '/ExPaginaErro': ExPaginaErro
  }

  // Obter o conteúdo a partir da cerquila, exemplo: http://localhost:5173/#/sobre o retorno será: #/sobre
  const referenciaRota = ref(window.location.hash)

  // Executa a ação quando realizar a navegação entre páginas. Obter o conteúdo a partir da cerquilha
  window.addEventListener('hashchange', () => {
    referenciaRota.value = window.location.hash
  });

  // Função responsável por exibir a página específica
  const currentView = computed(() => {
    return routes[referenciaRota.value.slice(1) || '/'] || ExPaginaErro
  })
</script>

<!-- TEMPLATE -->
<template>
  <!-- Links -->
  <a href="#/">ExPágina 1</a>
  |
  <a href="#/Expagina2">ExPágina 2</a>

  <!-- Exibição das páginas -->
  <component :is="currentView" />
</template>