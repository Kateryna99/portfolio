<script setup lang="ts">
import Header from "@/components/Header/Header.vue";
import Footer from "@/components/Footer/Footer.vue";
import Hero from "@/components/Hero/Hero.vue";
import Skills from "@/components/Skills/Skills.vue";
import Projects from "@/components/Projects/Projects.vue";
</script>

<template>
  <div class="wrapper">
    <Header />
    <div class="main">
      <Hero />
      <Skills />
      <Projects />
    </div>
    <Footer />
  </div>
</template>

<style scoped></style>
