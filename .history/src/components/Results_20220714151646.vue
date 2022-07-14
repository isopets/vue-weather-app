<template>
  <div v-if="results.country">{{ results.country }}</div>
  <div v-if="results.country">{{ results.cityName }}</div>
  <div v-if="results.country">{{ results.temperature }}</div>
  <div v-if="results.country">
    <img :src="results.icon" alt="icon" />
    <span>{{ results.conditionText }}</span>
  </div>
</template>

<script setup>
const props = defineProps({results: Object});
</script>
