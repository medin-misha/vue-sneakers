<script setup>

</script>

<template>
 <header class="border-slate-400 border-b flex justify-between">
  <div class="flex items-center gap-4 px-10 py-6">
    <img src="/logo.png" alt="лого" class="w-10"/>
    <div>
      <h2 class="text-xl font-bold">Sneakers</h2>
      <p class="text-slate-500">Ахуенные кросовки!</p>
    </div>
  </div>
  <div>
    <ul class="cursor-pointer flex items-center gap-10 py-8 px-10">
      <li class="flex item-center gap-2">
        <img src="/cart.svg" alt="стоимость корзины">
        <span class="text-gray-500 hover:text-gray-600">Стоимость корзины: 123.2</span>
      </li>
      <li class="cursor-pointer flex item-center gap-2">
        <img src="/heart.svg" alt="вкладки">
        <span class="text-gray-500 hover:text-gray-600">Закладки</span>
      </li>
      <li class="cursor-pointer flex item-center gap-2">
        <img src="/profile.svg" alt="профиль">
        <span class="text-gray-500 hover:text-gray-600">Профиль</span>
      </li>
    </ul>
  </div>
 </header>
</template>

<style scoped>

</style>
