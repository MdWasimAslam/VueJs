<script setup>
  const link = "https://google.com";
  const wallpaper = "https://thumbs.dreamstime.com/b/lonely-cherry-tree-seaside-rocks-d-artwork-35112983.jpg";
  const altText = "Amazing wallpaper";
  const imageWidth = "400px";
  const imageHeight = "250px"
</script>


<template>
  <a v-bind:href="link" > Google Link</a>
  <a :href="link">Google link 2</a>
  <img :src='wallpaper' :alt="altText" :width="imageWidth" :height="imageHeight">
</template>



<style>

</style>
