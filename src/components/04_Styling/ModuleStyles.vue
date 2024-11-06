<template>
  <h1>Module Styling</h1>

  <h2 :class="$style['m-1']">Module Styles 1</h2>
  <h2 :class="[$style['m-1'], $style['m-2']]">Module Styles 2</h2>
  <h2 :class="myModule.m3">Module Styles 3</h2>




</template>

<script setup>

</script>

<style module>
.m-1 {
  background-color: fuchsia;
}

.m-2 {
  font-size: 5vh;
}
</style>

<style module="myModule">
.m3 {
  background-color: royalblue;
}
</style>
