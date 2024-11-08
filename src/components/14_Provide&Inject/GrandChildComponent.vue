<script setup>
import { inject } from 'vue';

const name = inject('name');
const carsData = inject('carsData');
</script>

<template>
  <h1>Grand Child</h1>
  <h2>{{ name }}</h2>
  <!-- <h1>{{ carsData }}</h1> -->

  <ul v-for="(cars,index) in carsData" :key="index" >
    <li>{{ cars }}</li>
  </ul>
</template>



<style></style>
