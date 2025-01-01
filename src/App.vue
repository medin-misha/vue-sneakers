<script setup>
import CardComponent from './components/CardComponent.vue'
import HeaderComponent from './components/HeaderComponent.vue'
import SliderComponent from './components/SliderComponent.vue'
import ProductsComponent from './components/ProductsComponent.vue'
</script>

<template>
  <div class="
  w-11/12 h-screen
  m-auto p-3 my-8
  bg-slate-300
  rounded-xl
  shadow-2xl">
    <HeaderComponent />
    <SliderComponent />
    <ProductsComponent />
    <CardComponent />
  </div>
</template>

<style scoped></style>
