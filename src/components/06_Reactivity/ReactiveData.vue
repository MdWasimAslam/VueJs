<script setup>
import { reactive } from 'vue';

let initialState = reactive({
  count: 0
})



let rData = reactive({
  id: 8922,
  info: {
    name: 'wasi'
  }
})


function changeData() {
  rData.id = 1234;
  rData.info.name = 'Monty'
}
</script>


<template>
  <h1>Reactive Data</h1>
  <h1>{{ initialState.count }}</h1>
  <button @:click="initialState.count++">Increment</button>
  <button @:click="initialState.count--">Decrement</button>

  <br>
  <h1>{{ rData }}</h1>
  <button @:click="changeData">Change Data</button>
</template>



<style></style>
