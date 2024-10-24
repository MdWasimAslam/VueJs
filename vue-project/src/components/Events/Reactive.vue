<script setup>
    import {reactive} from 'vue';

    let initialState = reactive({
        count: 0
    });
    const increment = () => {
        initialState.count++;
    }
</script>


<template>
    <div>
        <h1>Reactive Component</h1>
        <h1>Count : {{ initialState.count }}</h1>
        <button @click="increment">Increment</button>
    </div>
</template>



<style>

</style>