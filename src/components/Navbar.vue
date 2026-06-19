<template>
  <nav class="navbar">
    <router-link to="/">Home</router-link>
    <router-link to="/about">About</router-link>
    <router-link to="/projects">Projects</router-link>
  </nav>
</template>

<style scoped>
.navbar {
  display: flex;
  gap: 20px;
  padding: 20px;
  background: #333;
}

a {
  color: white;
  text-decoration: none;
}

.router-link-active {
  color: yellow;
  font-weight: bold;
}
</style>