
<script setup>
import { ref } from 'vue';

const count = ref(0);

const increment = ()=> count.value++;
const decrement = ()=> count.value--;
</script>




<template>
  <h1>ComposableComponent</h1>
  <h1>Count : {{ count }}</h1>

  <button @click="increment">+</button>
  <button @click="decrement">-</button>
</template>


<style>

</style>
