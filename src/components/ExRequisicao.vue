<script setup>
// Vetor contendo as postagens
import { onMounted, ref } from 'vue'

let vetor = ref([])
let vetor2= ref([])
onMounted(() => {
    fetch('https://jsonplaceholder.typicode.com/posts')
        .then(retorno => retorno.json())
        .then(retorno => vetor.value = retorno)
})

onMounted(() => {
    fetch('https://jsonplaceholder.typicode.com/comments')
        .then(retorno => retorno.json())
        .then(retorno => vetor2.value = retorno)
    })
</script>

<template>
    <h1>Requisições</h1>
    <table>
        <tr v-for="v, index in vetor" :key="index">
            <td>{{ v.userId }}</td>
            <td>{{ v.id }}</td>
            <td>{{ v.title }}</td>
            <td>{{ v.body }}</td> 
        </tr>

        <tr v-for="v2, index in vetor2" :key="index">
            <td>{{ v2.userId }}</td>
            <td>{{ v2.name}}</td>
            <td>{{ v2.email }}</td>
            <td>{{ v2.body }}</td> 
        </tr>
    </table>
</template>