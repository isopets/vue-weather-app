<template><Title /><Form /></template>

<script setup>
import axios from "axios";
import Title from "./components/Title.vue";
import Form from "./components/Form.vue";

const getWeather = () => {
  axios.get(
    "http://api.weatherapi.com/v1/current.json?key=75a9ebd02b7d4a81b1a40652221407&q=London&aqi=no" .then(res => )　
  );
};
</script>
