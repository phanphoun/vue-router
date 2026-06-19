<template>
  <div>
    <h1>📁 Projects</h1>

    <ul>
      <li
        v-for="project in projects"
        :key="project.id"
      >
        <router-link
          :to="'/projects/' + project.id"
        >
          {{ project.title }}
        </router-link>
      </li>
    </ul>
  </div>
</template>

<script setup>
const projects = [
  {
    id: 1,
    title: 'Portfolio Website'
  },

  {
    id: 2,
    title: 'Todo App'
  },

  {
    id: 3,
    title: 'Blog Website'
  }
]
</script>