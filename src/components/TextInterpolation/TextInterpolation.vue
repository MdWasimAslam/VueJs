<script setup>
const greet = "Hello World";

function add(num1, num2) {
  return num1 + num2;
}



</script>

<template>
  <h1>{{ greet }}</h1>
  <h2>{{ 2 + 2 }}</h2>
  <h3>{{ add(2, 4) }}</h3>
</template>

<style></style>
