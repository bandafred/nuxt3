<script setup lang="ts">
const {data: posts} = await useAsyncData(() => $fetch('http://jsonplaceholder.typicode.com/posts'))

</script>

<template>
<h1>Posts</h1>
  <div v-for="post in posts">
    <nuxt-link :to='`/posts/${post.id}`'>
    <p>{{post.title}} <sup>{{post.id}}</sup></p>
    </nuxt-link>
  </div>
</template>

<style scoped>

</style>