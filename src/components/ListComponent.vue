<script setup>
import CardComponent from './CardComponent.vue';
</script>


<template>
<div class="grid grid-cols-4 gap-5 mt-8">
        <CardComponent title="Кроссовки для квадроберов" :price="12312" imgUrl="/sneakers/sneakers-1.jpg" :isFavorite="true" :isAddad="false"/>
        <CardComponent title="Кроссовки для квадроберов" :price="12312" imgUrl="/sneakers/sneakers-1.jpg" :isFavorite="false" :isAddad="true"/>
        <CardComponent title="Кроссовки для квадроберов" :price="12312" imgUrl="/sneakers/sneakers-1.jpg" :isFavorite="true" :isAddad="false"/>
        <CardComponent title="Кроссовки для квадроберов" :price="12312" imgUrl="/sneakers/sneakers-1.jpg" :isFavorite="false" :isAddad="true"/>
      </div>
</template>