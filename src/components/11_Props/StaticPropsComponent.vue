<script setup>
const props = defineProps(['name']);
console.log(props);


</script>


<template>
  <h1>Statis Props Component</h1>
  <h1>{{ props.name }}</h1>
</template>



<style></style>
