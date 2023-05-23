<script setup lang="ts">

</script>

<template>
  <nav class="nav">
    <h3>Nuxt App</h3>
    <ul>
      <li>
        <nuxt-link to="/">Home</nuxt-link>
      </li>
      <li>
        <nuxt-link to="/about">About</nuxt-link>
      </li>
      <li>
        <nuxt-link to="/posts">Posts</nuxt-link>
      </li>
    </ul>

  </nav>
</template>

<style scoped>

.nav {
  position: absolute;
  top: 0;
  left: 0;
  right: 0;
  height: 60px;
  padding: 0 2rem;
  display: flex;
  align-items: center;
  background: darkblue;
  justify-content: space-between;
}

ul {
  list-style: none;
  padding: 0;
  margin: 0;
  display: flex;
}

ul li {
  margin-right: 10px;
}

ul li a {
  color: aquamarine;
  text-decoration: none;
}

ul li a:hover {
  text-decoration: underline;
}
</style>