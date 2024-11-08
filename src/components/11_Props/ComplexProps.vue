<script setup>
defineProps({
  friends: Array,
  userInfo: Object
});


</script>

<template>
  <h1>Complex Validation</h1>
  <!-- <h2>{{ friends }}</h2>
  <h2>{{ userInfo }}</h2> -->

  <!-- Iterating over friends array  -->
  <ul v-for="(friend, index) in friends" :key="index">
    <li>{{ friend }}</li>
  </ul>

  <ul v-for="(info, index) in userInfo" :key="index">
    <li>{{ info }}</li>
  </ul>


</template>



<style></style>
