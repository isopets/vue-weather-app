<template>
  <div v-if="results.country">{{ results.country }}</div>
  // 追加
  <div v-if="results.cityName">{{ results.cityName }}</div>
  // 追加
  <div v-if="results.temperature">{{ results.temperature }}</div>
  // 追加
  <div v-if="results.icon">
    <img :src="results.icon" alt="icon" />
    <span>{{ results.conditionText }}</span>
  </div>
</template>

<script setup>
const props = defineProps({results: Object});
</script>
