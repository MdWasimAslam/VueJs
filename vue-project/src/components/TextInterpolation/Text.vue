<script setup>
const message = 'Text Interpolation';

function addTwoNumbers(a, b) {
    return a + b;
}


</script>



<template>
    <div>
        <h1>{{ message }}</h1>
        <h2> {{ addTwoNumbers(2, 6) }}</h2>
    </div>
</template>


<style></style>