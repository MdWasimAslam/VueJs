<script setup>
const imageInfo = {
  src: 'https://gratisography.com/wp-content/uploads/2024/03/gratisography-funflower-800x525.jpg',
  alt: 'Yello Flower',
  height: '250',
  width: '400'
}
</script>


<template>
  <h1>Dynamic Binding</h1>
  <img :src="imageInfo.src" :alt="imageInfo.alt" :height="imageInfo.height" :width="imageInfo.width">
</template>



<style></style>
