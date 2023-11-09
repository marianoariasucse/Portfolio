<template>
  <section id="about" class="w-full py-20 px-4 md:px-6 bg-gray-800">
    <h2 class="text-3xl sm:text-5xl font-bold text-center text-gray-200">Acerca de mí</h2>
    <div class="mt-8 max-w-3xl mx-auto grid gap-2 sm:grid-cols-2 items-center">
      <img :src="profileImage" width="320" height="320" alt="Imagen de perfil" class="mx-auto mb-4 rounded"
        style="aspect-ratio: 320 / 320; object-fit: cover;" />
      <div>
        <p class="text-lg sm:text-xl text-gray-400">
          {{ aboutMeParagraph }}
        </p>
      </div>
    </div>
    <SocialMediaNetworks />
  </section>
</template>

<script setup>
import { aboutMeParagraph, profileImage } from '../constants/ProfileInfo.js'
import SocialMediaNetworks from './SocialMediaNetworks.vue';
</script>