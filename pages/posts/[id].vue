<script setup lang="ts">
const route = useRoute()
let id = route.params.id;

const {data: post} = await useAsyncData(() => $fetch('http://jsonplaceholder.typicode.com/posts/' + id))

</script>

<template>
  <h1>POST</h1>
  
  <h3>{{post.title}}</h3>
  <h2>{{post.body}}</h2>
  <h3>{{post.id}}</h3>
</template>

<style scoped>

</style>