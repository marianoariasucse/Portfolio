<template>
  <section class="w-full py-60 px-4 md:px-6 bg-gradient-to-r from-green-400 to-blue-500 text-white text-center">
    <h1 class="text-4xl sm:text-6xl font-bold animate-bounce">Hola, soy {{ name }}</h1>
    <p class="mt-4 mx-auto text-xl sm:text-2xl">{{ title }}</p>
    <Button text="Ver Proyectos" variant="primary" @click="redirectToProjects" />
  </section>
</template>

<script setup>
import { name, title } from '../constants/ProfileInfo.js'
import Button from './Button.vue'

const redirectToProjects = () => {
  window.location.href = '/#projects'
}
</script>