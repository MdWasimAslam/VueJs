<script setup>
// Basically used for sending data from child to parent component
import { ref } from 'vue';
import ChildComponent from './ChildComponent.vue';


let count = ref(0);

</script>

<template>
  <h1>Component Events</h1>
  <h1>Count : {{ count }}</h1>
  <ChildComponent @incrementCount="count++" />
</template>

<style></style>
