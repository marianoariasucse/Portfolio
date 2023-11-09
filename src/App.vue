<template>
  <div class="flex flex-col min-h-screen bg-gray-900">
    <Header />
    <main class="flex-1">
      <HeroSection />
      <AboutMeSection />
      <SkillsSection />
      <ProjectsSection />
      <ContactSection />
    </main>
    <Footer />
  </div>
</template>

<script setup>
import Header from './components/Header.vue'
import HeroSection from './components/HeroSection.vue'
import AboutMeSection from './components/AboutMeSection.vue'
import SkillsSection from './components/SkillsSection.vue'
import ProjectsSection from './components/ProjectsSection.vue'
import ContactSection from './components/ContactSection.vue'
import Footer from './components/Footer.vue'
</script>