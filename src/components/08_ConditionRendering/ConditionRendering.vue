<script setup>
import { ref } from 'vue';


let isTrue = true;
let isFalse = true;

let isVisible = ref(true);


let isUserLoggedIn = ref(true);
let userName = 'Wasi';

let showDetails = ref(isUserLoggedIn)

</script>

<template>
  <h1>Condition Rendering</h1>
  <h2 v-if="isTrue">IsTrue is True</h2>
  <h2 v-if="isFalse">IsFalse is True</h2>
  <h2 v-else-if="true">This will show when isFalse is false</h2>
  <hr>

  <hr>

  <p v-show="isVisible" >Lorem ipsum dolor sit amet consectetur adipisicing elit. Laudantium, cumque.</p>
  <button @:click="isVisible = !isVisible">Toggle</button>

  <br>
  <hr>

  <h1 v-if="isUserLoggedIn">Welcome, {{ userName }}</h1>
  <h1 v-else>Please Login</h1>
  <button @:click="showDetails = false">logout</button>
</template>



<style></style>
