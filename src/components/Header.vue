<template>
  <header class="px-4 lg:px-6 h-16 flex items-center justify-between bg-gray-800 shadow-md">
    <div class="flex items-center space-x-4">
      <a class="flex gap-3 cursor-pointer" href="/">
        <svg xmlns="http://www.w3.org/2000/svg" width="24" height="24" viewBox="0 0 24 24" fill="none" stroke="currentColor"
        stroke-width="2" stroke-linecap="round" stroke-linejoin="round" class=" h-8 w-8 text-blue-300">
        <polyline points="16 18 22 12 16 6"></polyline>
        <polyline points="8 6 2 12 8 18"></polyline>
      </svg>
      <span class="text-lg font-semibold text-gray-200">{{ name }}</span>
      </a>
    </div>
    <nav class="hidden md:flex gap-4 items-center">
      <a class="text-sm font-medium text-gray-400 hover:text-blue-400" href="#about">
        Acerca de
      </a>
      <a class="text-sm font-medium text-gray-400 hover:text-blue-400" href="#skills">
        Habilidades
      </a>
      <a class="text-sm font-medium text-gray-400 hover:text-blue-400" href="#projects">
        Proyectos
      </a>
      <a class="text-sm font-medium text-gray-400 hover:text-blue-400" href="#contact">
        Contacto
      </a>
      <Button text="Descargar CV" variant="secondary" @click="downloadCV" />
    </nav>
  </header>
</template>

<script setup>
import { name } from '../constants/ProfileInfo.js'
import Button from './Button.vue'

const downloadCV = () => {
  const pdfPath = '/assets/portfolioCV.pdf';
  const link = document.createElement('a');
  link.href = pdfPath;
  link.download = 'CV.pdf';
  link.click();
}
</script>