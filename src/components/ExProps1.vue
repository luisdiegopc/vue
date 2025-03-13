<script setup>
// importar componentes
import ExProps2 from './ExProps2.vue';
let cidade = 'São Paulo'
let cidades = ['São Paulo', 'Rio de Janeiro', 'Fortaleza', 'Recife']
 
</script>

<template> 

<ExProps2 nome="Ralf" idade="33" :cidade="cidade" :vetor="cidades"> </ExProps2>
</template>