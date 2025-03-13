<script setup>
function mensagem() {
        alert('Trab com eventos de clique!')
    }
</script>

<template>
    <button @click="mensagem">Clique</button>
</template>