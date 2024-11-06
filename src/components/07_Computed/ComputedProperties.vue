<script setup>
import { ref, computed } from 'vue';

let num = ref(5)

const sqauredNum = computed(() => {
  return num.value * num.value;
})

let fName = 'Wasim';
let lName = 'Aslam';

let fullName = computed(() => {
  return fName + ' ' + lName
})


</script>

<template>
  <h1>Computed Properties</h1>
  <h1>Orginal Num : {{ num }}</h1>
  <h1>Sqared Num : {{ sqauredNum }}</h1>

  <br>
  <h1>
    firstName : {{ fName }}
  </h1>
  <h1>
    lastName : {{ lName }}
  </h1>
  <h1>
    fullName : {{ fullName }}
  </h1>

</template>



<style></style>
