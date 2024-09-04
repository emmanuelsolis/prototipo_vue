<script setup>
import { RouterView } from 'vue-router'
import Header from '/src/components/Header.vue'
import Footer from '/src/components/Footer.vue'
</script>

<template>
  <Header></Header>

  <RouterView />
  <Footer></Footer>
</template>

<style scoped></style>
