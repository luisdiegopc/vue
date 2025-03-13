<script setup>
let nomes = ['Aline', 'Bruna', 'Ana Paula', 'Karol'];
</script>

<template>
 <li v-for="nome in nomes" :key="nome.name" >
  {{ nome }}
</li>
</template>