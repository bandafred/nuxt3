<script setup lang="ts">
const {data: user} = await useAsyncData(() => $fetch('/api/user'))

function first(){
  let count = 0;
  return { 
    inner() {
      return count++;
    }
  }
}

let d = first();
console.log('count', d.inner());
console.log('count', d.inner());
console.log('count', d.inner());
console.log('count', d.inner());


</script>

<template>
 <h1>Home</h1>
  <pre>{{ user }}</pre>
</template>

<style scoped>

</style>