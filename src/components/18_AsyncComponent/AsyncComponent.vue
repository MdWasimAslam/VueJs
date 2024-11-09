
<script setup>
  import { defineAsyncComponent, ref } from 'vue';
  // import MovieData from './MovieData.vue';

  const MovieData = defineAsyncComponent(()=> import('./MovieData.vue')) // <--- Now when the component is required then only it will be mounted
  const showData = ref(false);
</script>




<template>
  <h1>Async</h1>
  <MovieData v-if="showData"/>
  <button @click="showData=!showData">Toggle Data</button>
</template>


<style>

</style>
