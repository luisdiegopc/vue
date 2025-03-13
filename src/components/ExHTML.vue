<script setup>
// let texto = 'Aprendendo a Diretiva v-HTML'
 let texto = '<p style="color:red; font-size:33px; font-weight:bold"> Aprendendo a directiva V-HTML. </p>'
</script>

<template>
    <div v-html="texto"> </div>
    <div> {{ texto }}</div>
</template>
 