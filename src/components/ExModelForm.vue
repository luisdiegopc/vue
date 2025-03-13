<script setup>
    // Variável reativa, tudo que digitar no htlm vai aparecer logo a baixo! 
    import { ref } from 'vue'

    let texto =    ref ('')  
</script>

<template>
    <input type="text" v-model="texto"> 
    <p>{{ texto }}</p>
</template>