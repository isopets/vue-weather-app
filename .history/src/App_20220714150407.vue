<template><Title /><Form @submit-form="getWeather" /> <Results /></template>

<script setup>
import {reactive} from "vue";
import axios from "axios";
import Title from "./components/Title.vue";
import Form from "./components/Form.vue";
import Results from "./components/Results.vue";

const results = reactive({
  country: "",
  cityName: "",
  temperature: "",
  conditionText: "",
  icon: "",
});

const getWeather = () => {
  axios
    .get(
      "http://api.weatherapi.com/v1/current.json?key=75a9ebd02b7d4a81b1a40652221407&q=London&aqi=no"
    )
    .then(res => console.log(res));
};
</script>
