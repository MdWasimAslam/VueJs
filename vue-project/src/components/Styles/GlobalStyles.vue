<template>
    <div>
        <h1 class="text-red">Global Styling</h1>
        <p class="local">Trying local scope in this element</p>
    </div>
</template>



<!-- Global Styles -->
<!-- scoped is used to remove global styling and just use the styles locally -->

<style >
/* <style scoped> */
.text-red {
    color: red;
}
</style>