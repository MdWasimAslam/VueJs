<script setup>

  let fruits = ['Apple','Mango','Banana','Guava','Oranges']
</script>


<template>
  <h1>V-FOR</h1>
  <h2 v-for="(fruit,index) in fruits" :key="index">{{ fruit }}</h2>
</template>



<style>

</style>
