<script setup>
import { onMounted, ref } from 'vue';

const myref = ref('Wasi');
console.log(myref.value)
onMounted(() => {
  console.log(myref.value)
  myref.value.focus() // ref directly selects the dom element and then we can maniplate as per required
})
</script>




<template>
  <h1>template Ref</h1>
  <input ref="myref" placeholder="Something..." />
</template>


<style></style>
