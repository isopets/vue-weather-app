<template>
  <div class="results-country" v-if="results.country">
    {{ results.country }}
  </div>
  <div class="results-city" v-if="results.cityName">{{ results.cityName }}</div>
  <div class="results-temp" v-if="results.temperature">
    {{ results.temperature }}
  </div>
  <div class="results-condition" v-if="results.icon">
    <img :src="results.icon" alt="icon" />
    <span>{{ results.conditionText }}</span>
  </div>
</template>

<script setup>
import {toRefs} from "vue";
const {country, cityName, temperature, icon, conditionText} = toRefs(
  props.results
);
</script>
