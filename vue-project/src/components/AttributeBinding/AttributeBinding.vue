<template>
    <div>
        <h1>Attribute Binding</h1>
        <!-- Old way -->
        <a v-bind:href="link">Google</a>
        <!-- New way -->
        <a :href="link">Google</a>

        <img :src="googleLogo" :alt="altText" :height="imageHeight" :width="imageWidth">


        <!-- Dynamic Attribute Binding -->
        <!-- <img :src="imageInfo.src" :alt="imageInfo.alt" :height="imageInfo.height" :width="imageInfo.width"> -->
        <img v-bind="imageInfo">
    </div>
</template>

<script setup>
const link = 'https://www.google.com';

const googleLogo = 'https://www.google.com/images/branding/googlelogo/1x/googlelogo_color_272x92dp.png';
const altText = 'Google Logo';
const imageWidth = 100;
const imageHeight = 35;


// Dynamic Attribute Binding
    const imageInfo = {
        src: 'https://cdn.logojoy.com/wp-content/uploads/20230921104407/Facebook-logo-2015_2019-600x319.png',
        alt: 'Facebook Logo',
        width: 100,
        height: 100
    }

</script>

<style></style>