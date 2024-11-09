<script setup>
import { ref, onBeforeMount, onMounted, onUpdated, onBeforeUnmount, onUnmounted, onBeforeUpdate } from 'vue';

let message = ref('Hello, Vue!');

onBeforeMount(() => {
  console.log('Component is about is to be mounted...')
})


onMounted(() => {
  console.log('Component has been mounted!')
})

onBeforeUpdate(() => {
  console.log('Component is about to be updated!')
})


onUpdated(() => {
  console.log('Component has been updated!')
})



function updateMsg() {
  message.value = "Hello Wasim"
}
</script>


<template>

  <h1>Life Cycle</h1>
  <p>{{ message }}</p>
  <button @click="updateMsg">Update Message</button>
</template>
