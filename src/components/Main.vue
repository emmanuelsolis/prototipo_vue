<template>
  <main class="container mx-auto px-4 py-12">
    <h2 class="text-3xl font-bold mb-8 text-center">Nuestros Proyectos de Movilidad Limpia</h2>
    <div class="grid grid-cols-1 md:grid-cols-2 lg:grid-cols-3 gap-8">
      <div
        v-for="project in projects"
        :key="project.id"
        class="bg-white rounded-lg shadow-md overflow-hidden"
      >
        <img :src="project.image" :alt="project.title" class="w-full h-48 object-cover" />
        <div class="p-6">
          <h3 class="text-xl font-semibold mb-2">{{ project.title }}</h3>
          <p class="text-gray-600 mb-4">{{ project.description }}</p>
          <a href="#" class="text-green-500 hover:text-green-600 transition-colors">Leer más</a>
        </div>
      </div>
    </div>
  </main>
</template>

<script setup>
import { ref } from 'vue'

const projects = ref([
  {
    id: 1,
    title: 'Coche Eléctrico Autónomo',
    description: 'Un vehículo eléctrico con capacidades de conducción autónoma y cero emisiones.',
    image: '/placeholder.svg?height=300&width=400'
  },
  {
    id: 2,
    title: 'Aeronave de Hidrógeno',
    description:
      'Una aeronave propulsada por hidrógeno para vuelos de corta distancia sin emisiones.',
    image: '/placeholder.svg?height=300&width=400'
  },
  {
    id: 3,
    title: 'Bicicleta Eléctrica Plegable',
    description:
      'Una bicicleta eléctrica compacta y plegable para desplazamientos urbanos eficientes.',
    image: '/placeholder.svg?height=300&width=400'
  }
])
</script>
