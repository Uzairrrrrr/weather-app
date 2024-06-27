<template>
  <footer class="bg-weather-primary py-4">
    <div class="container mx-auto text-center text-white text-opacity-50">
      <p class="mb-2">
        © {{ currentYear }} All rights reserved to <span class="font-semibold">Uzair</span>.
      </p>
    </div>
  </footer>
</template>

<script setup>
import { ref, onMounted } from "vue";

const currentYear = ref(new Date().getFullYear());

onMounted(() => {
  currentYear.value = new Date().getFullYear();
});
</script>
