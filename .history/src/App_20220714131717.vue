<template><Title /><Form /></template>

<script setup>
import axios from "axios";
import Title from "./components/Title.vue";
import Form from "./components/Form.vue";

const getWeather = () => {
  axios.get("");
};
</script>

