<script setup>
  defineProps({
    name:{
      type:String,
      validator:(propsVal)=>{
        return ['Huxn','Wasi','John'].includes(propsVal)
      }
    },
    age:{
      type:Number,
      validator:(propVal)=>(propVal>=18 && propVal <= 30 ? true : false)
    },
    password:{
      type:String,
      validator:(propVal)=>propVal.length >=8
    }
  })
</script>

<template>
  <h1>Custom Validator</h1>
  <h1>{{ name }}</h1>
  <h1>{{ age }}</h1>
  <h1>{{ password }}</h1>
</template>



<style></style>
