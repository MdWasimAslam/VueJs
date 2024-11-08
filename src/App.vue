<script setup>

// import ParentComponent from './components/NestedComponents/ParentComponent.vue';
// import TextInterpolation from './components/TextInterpolation/TextInterpolation.vue';
// import AttributeBinding from './components/Binding/AttributeBinding.vue';
// import DynamicBinding from './components/Binding/DynamicBinding.vue';
// import GlobalStyles from './components/04_Styling/GlobalStyles.vue';
// import ModuleStyles from './components/04_Styling/ModuleStyles.vue';
// import Event from './components/05_Events/Events_.vue';
// import ReactiveData from './components/06_Reactivity/ReactiveData.vue';
// import RefData from './components/06_Reactivity/RefData.vue';
// import ComputedProperties from './components/07_Computed/ComputedProperties.vue';
// import ConditionRendering from './components/08_ConditionRendering/ConditionRendering.vue';
// import vFor from './components/09_V-For/vFor.vue';
// import VModel from './components/10_vModel/vModel.vue';
// import StaticPropsComponent from './components/11_Props/StaticPropsComponent.vue';
// import DynamicPropsComponent from './components/11_Props/DynamicPropsComponent.vue';
// //----- Dynamiv Value -----
// const name = "Wasim";

// import { ref } from 'vue';
// import ChangingProps from './components/11_Props/ChangingProps.vue';
// const favNum = ref(3);

// import PropsValidation from './components/11_Props/PropsValidation.vue';
// import ComplexProps from './components/11_Props/ComplexProps.vue';
import CustomValidator from './components/11_Props/CustomValidator.vue';
</script>



<template>
  <h1>App Component</h1>
  <!-- <ParentComponent/> -->
  <!-- <TextInterpolation/> -->
  <!-- <AttributeBinding/> -->
  <!-- <DynamicBinding /> -->
  <!-- <GlobalStyles /> -->
  <!-- <ModuleStyles /> -->
  <!-- <Event/> -->
  <!-- <ReactiveData/> -->
  <!-- <RefData/> -->
  <!-- <ComputedProperties/> -->
  <!-- <ConditionRendering/> -->
  <!-- <vFor/> -->
  <!-- <VModel/> -->
  <!-- <StaticPropsComponent name="Wasi"/> -->
  <!-- <DynamicPropsComponent :name="name"/> -->
  <!-- <ChangingProps :favNum="favNum"/> -->
  <!-- <PropsValidation name="jordan" :age="5"/> -->
  <!-- <ComplexProps
  :friends="['alex', 'john', 'harley']"
  :userInfo="{name:'alex',age:20,location:['Earth','IDK']}"
  /> -->

  <CustomValidator name="Wasism" :age="2433" password="555"/>
  <Props />
</template>



<style></style>
