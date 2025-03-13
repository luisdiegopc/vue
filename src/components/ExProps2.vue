<script setup>
//Obter Props
import { defineProps } from 'vue';
 let props = defineProps(['nome', 'idade', 'vetor'])
// variáveis

 
</script>

<template> 

    <h1>Nome: {{ props.nome }}</h1>
    <h1>Idade: {{ props.idade }}</h1>
    <p>Cidade: {{  cidades }}</p>

    <ul>
        <li v-for="(vetor,  index) in vetor" :key="index">{{ vetor }}</li>
    </ul>
</template>