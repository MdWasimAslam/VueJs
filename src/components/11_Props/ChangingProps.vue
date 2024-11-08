<script setup>
  const props = defineProps(['favNum']);

  console.log(props)
  // props.favNum = 10; <--- Will not work props value cannot be changed
</script>

<template>
  <h1>Changing Props Value</h1>
  <h1>{{ props.favNum }}</h1>
</template>



<style></style>
