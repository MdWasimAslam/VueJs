<script setup>
import { ref } from 'vue';

const formData = ref({
  username: '',
  email: '',
  password: ''
})

let isLoggedIn = ref(false)

const login = () => {
  if (formData.value.username === 'wasi' && formData.value.password === 'wasi') {
    isLoggedIn.value = true
  }
}
</script>



<template>
  <h1>v Model</h1>
  <input type="text" placeholder="Please enter username" v-model="formData.username">
  <!-- <input type="text" placeholder="Please enter email" v-model="formData.email"> -->
  <input type="text" placeholder="Please enter password" v-model="formData.password">

  <h2>{{ formData.username }}</h2>
  <h2>{{ formData.email }}</h2>
  <h2>{{ formData.password }}</h2>

  <button @click="login">Login</button>

  <br>
  <br>

  <div v-if="isLoggedIn">Lorem ipsum, dolor sit amet consectetur adipisicing elit. Mollitia velit, expedita eum error
    numquam tenetur debitis recusandae voluptates voluptas? Laboriosam?</div>
</template>



<style></style>
