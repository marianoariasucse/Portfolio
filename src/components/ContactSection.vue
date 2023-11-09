
import SocialMediaNetworks from './SocialMediaNetworks.vue';
<template>
  <section id="contact" class="w-full py-20 px-4 md:px-6 bg-gray-800">
    <h2 class="text-3xl sm:text-5xl font-bold text-center text-gray-200">Contacto</h2>
    <form class="mt-8 max-w-xl mx-auto grid gap-4">
      <input
        class="flex h-10 w-full border px-3 py-2 text-sm ring-offset-background file:border-0 file:bg-transparent file:text-sm file:font-medium placeholder:text-muted-foreground focus-visible:outline-none focus-visible:ring-2 focus-visible:ring-ring focus-visible:ring-offset-2 disabled:cursor-not-allowed disabled:opacity-50 rounded-md border-gray-700 focus:border-blue-400 focus:ring-1 focus:ring-blue-400 bg-gray-900 text-gray-200"
        placeholder="Nombre" type="text" />
      <input
        class="flex h-10 w-full border px-3 py-2 text-sm ring-offset-background file:border-0 file:bg-transparent file:text-sm file:font-medium placeholder:text-muted-foreground focus-visible:outline-none focus-visible:ring-2 focus-visible:ring-ring focus-visible:ring-offset-2 disabled:cursor-not-allowed disabled:opacity-50 rounded-md border-gray-700 focus:border-blue-400 focus:ring-1 focus:ring-blue-400 bg-gray-900 text-gray-200"
        placeholder="Correo electrónico" type="email" />
      <input
        class="flex w-full border px-3 py-2 text-sm ring-offset-background file:border-0 file:bg-transparent file:text-sm file:font-medium placeholder:text-muted-foreground focus-visible:outline-none focus-visible:ring-2 focus-visible:ring-ring focus-visible:ring-offset-2 disabled:cursor-not-allowed disabled:opacity-50 rounded-md border-gray-700 focus:border-blue-400 focus:ring-1 focus:ring-blue-400 bg-gray-900 text-gray-200 h-32"
        as="textarea" placeholder="Mensaje" />
      <button
        class="inline-flex items-center justify-center text-sm font-medium ring-offset-background transition-colors focus-visible:outline-none focus-visible:ring-2 focus-visible:ring-ring focus-visible:ring-offset-2 disabled:pointer-events-none disabled:opacity-50 h-10 mt-4 px-8 py-2 bg-blue-500 hover:bg-gray-700 text-white rounded-md"
        type="submit">
        Enviar mensaje
      </button>
    </form>
    <SocialMediaNetworks />
  </section>
</template>

<script setup>
import SocialMediaNetworks from './SocialMediaNetworks.vue';
</script>