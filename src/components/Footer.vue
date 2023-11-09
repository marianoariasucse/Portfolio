<template>
    <footer class="py-3 flex items-center justify-center bg-gray-900 shadow-md">
        <p class="text-white">© {{ actualYear }} - Mariano Arias Portafolio</p>
    </footer>
</template>

<script setup>
const actualYear = new Date().getFullYear()
</script>