<script setup>
  import Parent from './components/components/Parent.vue';
  import Text from './components/TextInterpolation/Text.vue';
  import AttributeBinding from './components/AttributeBinding/AttributeBinding.vue';
  import GlobalStyles from './components/Styles/GlobalStyles.vue';
  import LocalStyles from './components/Styles/LocalStyles.vue';
  import CombinedStyles from './components/Styles/CombinedStyles.vue';
  import ModuleStyles from './components/Styles/ModuleStyles.vue';
  import Event from './components/Events/Event.vue';
  import Reactive from './components/Events/Reactive.vue';
</script>

<template>
  <div>
    <h1>App Component</h1>
    <!-- <Parent/> -->
     <!-- <Text/> -->
    <!-- <AttributeBinding/> -->
     <!-- <GlobalStyles/>
     <LocalStyles/>
     <CombinedStyles/>  
     <ModuleStyles/> -->

      <!-- <Event/> -->
      <Reactive/>
  </div>

</template>

<style scoped></style>