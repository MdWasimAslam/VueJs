<script setup>
import LocalStyles from './LocalStyles.vue';
</script>

<template>
  <h1 class="text-red">Parent Component</h1>
  <h2 class="global">Global Styling here</h2>
  <h3 class="scoped">Scoped Parent</h3>
  <LocalStyles/>
</template>


<style>
.text-red {
  color: red
}
.global{
  color:orange
}
</style>


<style scoped>
  .scoped{
    color: darkolivegreen
  }
</style>

