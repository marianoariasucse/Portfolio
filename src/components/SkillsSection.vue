<template>
  <section id="skills" class="w-full py-20 px-4 md:px-6 bg-gray-900">
    <h2 class="text-3xl sm:text-5xl font-bold text-center text-gray-200">Habilidades</h2>
    <div class="mt-8 grid gap-4 sm:grid-cols-2 lg:grid-cols-4">
      <div v-for="skill in skills"
        class="flex items-center gap-3 bg-gray-800 shadow-md rounded-md p-4 transition-transform duration-500 ease-in-out transform hover:scale-105">
        <img :src="skill.icon" class="w-16 h-16" />
        <h3 class="text-xl font-medium text-gray-200">{{ skill.name }}</h3>
      </div>
    </div>
  </section>
</template>

<script setup>
import { skills } from '../constants/ProfileInfo';
</script>