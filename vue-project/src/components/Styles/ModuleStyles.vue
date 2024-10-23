<template>
  <div>
    <!-- <h1 :class="$style['m-class']"> Using Module Styling</h1> -->
    <h1 :class="MyClasses['m2-class']"> Using Module Styling</h1>
  </div>
</template>



<style module="MyClasses">
    .m-class{
        color: rgb(1, 255, 56);
        background: black;
    }
    .m2-class{
        color: rgb(1, 221, 255);
        background: black;
    }
</style>