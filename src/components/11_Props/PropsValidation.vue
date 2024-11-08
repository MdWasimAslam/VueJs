<script setup>
// const props = defineProps({
//   name: String,
//   age: Number
// });
// console.log(props)


// Advance Props Validation

const props = defineProps({
  names: {
    type: String,
    required: true,
    default:'Anonymous'
  }
})

console.log(props)

</script>

<template>
  <h1>Props Validation</h1>
</template>



<style></style>
