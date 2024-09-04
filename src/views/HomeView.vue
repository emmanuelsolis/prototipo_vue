<template>
  <div class="home-view">
    <Banner />
    <Main />
  </div>
</template>

<script setup>
import Banner from '/src/components/Banner.vue'
import Main from '/src/components/Main.vue'
</script>

<style scoped>
.home-view {
  font-family: 'Arial', sans-serif;
  color: #333;
  line-height: 1.6;
}
</style>
