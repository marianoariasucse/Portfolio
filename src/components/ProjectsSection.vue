<template>
  <section id="projects" class="w-full py-20 px-4 md:px-6 bg-gray-900">
    <h2 class="text-3xl sm:text-5xl font-bold text-center text-gray-200">Proyectos</h2>
    <div class="mt-8 grid gap-8 sm:grid-cols-2 lg:grid-cols-3">
      <div v-for="project in ProjectsMade" key="project.title"
        class="bg-gray-800 shadow-md rounded-md p-4 mb-4 transition-transform duration-500 ease-in-out transform hover:scale-105">
        <img :src="project.image" width="200" height="120" alt="Proyecto 1" class="mx-auto mb-4 w-full" loading="lazy"
          style="aspect-ratio: 120/ 120; object-fit: cover;" />
        <h3 class="text-xl font-medium text-gray-200">{{ project.title }}</h3>
        <p class="mt-2 mb-4 text-sm text-gray-400">{{ project.description }}</p>
        <div class="flex gap-2 mb-3 items-center">
          <p class="text-gray-100">Tecnologias usadas: </p>
          <p class="mt-2 mb-4 text-sm text-gray-200 bg-gray-600 p-1 rounded" v-for="tecnology in project.tecnologies">
            {{ tecnology }}
          </p>
        </div>
        <div class="flex justify-between items-center">
          <div class="flex gap-2">
            <Button text="Vista Previa" variant="secondary" />
            <Button text="Ver Codigo" variant="tertiary" />
          </div>
          <p class="text-gray-200">{{ project.state }}</p>
        </div>
      </div>
    </div>
  </section>
</template>

<script setup>
import Button from './Button.vue'
import { ProjectsMade } from '../constants/ProjectsMade.js'
</script>