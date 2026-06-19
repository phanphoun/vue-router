<template>
  <div>
    <h1>📄 Project Detail</h1>

    <h2>{{ project.title }}</h2>

    <p>{{ project.description }}</p>
  </div>
</template>

<script setup>
import { useRoute } from 'vue-router'

const route = useRoute()

const projects = [
  {
    id: 1,
    title: 'Portfolio Website',
    description: 'A personal portfolio built using Vue.'
  },

  {
    id: 2,
    title: 'Todo App',
    description: 'A task management application.'
  },

  {
    id: 3,
    title: 'Blog Website',
    description: 'A blogging platform created with Vue.'
  }
]

const project = projects.find(
  p => p.id === Number(route.params.id)
)
</script>