<template>
  <Navbar />

  <main class="container">
    <router-view />
  </main>
</template>

<script setup>
import Navbar from './components/Navbar.vue'
</script>

<style>
body {
  margin: 0;
  font-family: Arial, sans-serif;
}

.container {
  padding: 30px;
}
</style>