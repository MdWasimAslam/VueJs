<script setup>
import { ref } from 'vue';
import { reactive } from 'vue';


let count = ref(0);
let users = ref(['Micheal','Zayn','Johnny']);

let info = ref({
  name:'Alex',
  location:{
    city:'New York'
  }
})


let fruits = reactive([ref('Banana'),ref('Mango')]);



</script>



<template>
  <h1>Ref</h1>
  <h1>{{ count }}</h1>
  <button @:click="count++">+</button>
  <button @:click="count--">-</button>
<br>
<h1>{{ users }}</h1>
<button @:click="users.push('Lionel')">Push User</button>


<br>
<h1>{{ info }}</h1>
<button @:click="info.location.city='Georia'">Update Location</button>

<br>

<h1>
{{ fruits }}
</h1>
<button @:click="fruits.push('Pineapple')">AddFruit</button>
<button @:click="fruits[fruits.length-1]='Guava'">Update Last Fruit</button>
</template>



<style>

</style>
