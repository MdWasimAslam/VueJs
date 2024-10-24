<script setup>
import { ref } from 'vue';


    const count = ref(0);
    const increment = () => {
        count.value++;
    }

    const decrement = () => {
        count.value--;
    }
    const submitHandler=(e)=>{
        e.preventDefault();
        console.log(e.target[0].value);
    }

    const showMessage=(msg)=>{
        alert(msg);
    }

</script>



<template>
    <div>
        <h1>Event Component</h1>
        <h1>Count : {{ count }}</h1>
        <button @:click="increment">Increment</button>
        <button @:click="decrement">Decrement</button>
        
        <form @submit="submitHandler">
            <input type="text"  />
            <button type="submit">Submit</button>
        </form>

        <button @click="()=>{console.log('Hello World')}">Click Me</button>
        <button @click="showMessage('Hello World')">Alert Btn</button>
    </div>
</template>



<style></style>