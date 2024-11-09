<script setup>
import { ref, watch } from 'vue';

const message = ref("Hello, Vue!");
const inputText = ref('');

// Watch for changes
watch(inputText, (newVal, oldVal) => {
  // You can perform some logic when input is changed
  console.log('Input changed:', newVal, oldVal);
  message.value = newVal
})
//--------- example 2 ------------


const count = ref(0);
const username = ref('Alex');


watch([count,username],(newVal,oldVal)=>{
  console.log('NewValue ---->',  newVal)
  console.log('OldValue ---->',  oldVal)
  console.log('---------------------------')
})

</script>




<template>
  <h1>Watcher</h1>
  <h1>{{ message }}</h1>
  <input v-model="inputText" placeholder="Type something...">
  <br>
  <hr/>

<h1>{{ count }}</h1>
<h1>{{ username }}</h1>
<button @click="count++">Increment</button>
<button @click="username='jordan'">change user</button>
</template>


<style></style>
