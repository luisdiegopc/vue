<script setup>
import { onMounted, ref } from 'vue'
let texto = ref('Hello Word!')

// Executa a msg e depois de 3 segundos ele muda 
onMounted(() => {
    setTimeout(() => {
        texto.value = 'Alterando texto'
    }, 3000)
})
</script>

<template>
    <h1>{{  texto }}</h1>
</template>