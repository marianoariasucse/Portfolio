<template>
    <!-- social media links -->
    <div class="mt-8 flex justify-center space-x-6">
        <a v-for="socialNetwork in socialNetworks" :key="socialNetwork.name" :href="socialNetwork.url" target="_blank"
            class="text-gray-400 hover:text-gray-200">
            <span class="sr-only">{{ socialNetwork.name }}</span>
            <img :src="socialNetwork.icon" width="40" :alt="socialNetwork.name + 'Icon'" :title="socialNetwork.name">
        </a>
    </div>
</template>

<script setup>
import { socialNetworks } from '../constants/ProfileInfo.js'
</script>