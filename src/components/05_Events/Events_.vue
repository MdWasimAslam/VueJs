<script setup>
import { ref } from 'vue';
const count = ref(0);


function increment() {
  count.value = count.value + 1;
}


function decrement() {
  count.value = count.value - 1;
}

function reset() {
  count.value = 0;
}
</script>


<template>
  <h1>Events</h1>
  <h1>{{ count }}</h1>
  <button v-on:click="count++">Increment</button>
  <button @:click="count--">Decrement</button>
  <br>
  <button @:click="increment" class="btn green">Increment Func</button>
  <button @:click="decrement" class="btn blue">Decrement Function</button>
  <button @:click="reset" class="btn purple">Reset</button>

</template>



<style>
.btn {
  color: white;
  padding: 10px 20px;
  margin-right: 10px;
  margin-top: 10px;
  border: none;
  cursor: pointer;
}

.green {
  background-color: rgb(2, 178, 84);

}

.blue {
  background-color: cadetblue;
}

.purple {
  background-color: purple;
}
</style>
