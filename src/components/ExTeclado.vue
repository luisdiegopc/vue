<script setup>
function mensagem() {
        alert('Exemplo de mensagem!')
    }
</script>

<template>

    <input type="text" @keyup.enter="mensagem">
</template>