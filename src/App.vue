<script setup>
import { useMonitor } from '@/composables/monitor';
import RodapeMobile from './components/RodapeMobile.vue';
const { menu } = useMonitor();
</script>

<template>
  <div>
    <component :is="menu" />
    <main>
      <router-view />
    </main>
    <footer>
      <p>Copyright &copy; 2024</p>
    </footer>
  </div>
  <RodapeMobile />
</template>

<style scoped>
</style>
