<script setup>
import ListComponent from './components/ListComponent.vue';
import HeaderComponent from './components/HeaderComponent.vue'

</script>

<template>
  <div class="
  w-11/12 
  m-auto my-8
  bg-slate-300
  rounded-xl
  shadow-2xl">
    <header-component/>
    <div class="p-10">
      <h2 class="text-3xl font-bold">Все Кроссовки</h2>
      <ListComponent/>
    </div>
      
  </div>
</template>

<style scoped></style>
