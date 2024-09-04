<template>
  <header class="header">
    <nav class="container mx-auto px-4 py-6 flex justify-between items-center">
      <div class="logo">
        <!-- <img src="/placeholder.svg?height=40&width=40" alt="Clean Mobility Logo" class="h-10" /> -->
      </div>
      <ul class="flex space-x-6">
        <li>
          <RouterLink class="hover:text-green-500 transition-colors" to="/">Inicio</RouterLink>
        </li>
        <li>
          <RouterLink class="hover:text-green-500 transition-colors" to="/about"
            >Nosotros</RouterLink
          >
        </li>
        <li>
          <RouterLink class="hover:text-green-500 transition-colors" to="/services"
            >Servicios</RouterLink
          >
        </li>
        <li>
          <RouterLink class="hover:text-green-500 transition-colors" to="/contact"
            >Contacto</RouterLink
          >
        </li>
      </ul>
    </nav>
  </header>
</template>

<script setup>
import { RouterLink } from 'vue-router'
</script>

<style scoped>
.header {
  background-color: #ffffff;
  box-shadow: 0 2px 4px rgba(0, 0, 0, 0.1);
}
</style>
