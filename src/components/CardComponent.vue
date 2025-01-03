<script setup>
import { ref } from 'vue';

// Декларация пропсов
const props = defineProps({
    imgUrl: String,
    title: String,
    price: Number,
    isFavorite: Boolean,
    isAddad: Boolean
});
// Переменные
const noLiked = "/like-1.svg";
const liked = "/like-2.svg";
const checked = "/checked.svg";
const plus = "/plus.svg";
var likePath = props.isFavorite == true ? ref(liked) : ref(noLiked)
var plusPath = props.isAddad == true ? ref(checked) : ref(plus);

const likedIt = (event) => {
    likePath.value = likePath.value == noLiked ? liked : noLiked;
}
const addadIt = (event) => {
    plusPath.value = plusPath.value == checked ? plus : checked
}
</script>

<template>
    <div class="
        bg-white 
        w-full min-w-32 р-full 
        p-3
        border border-red-400 rounded-lg
        relative
        drop-shadow-sm 
        
        hover:drop-shadow-xl
        hover:-translate-y-1
        transition
    ">
        <img :src="likePath" alt="like" @click="likedIt" class="w-1.5/5 absolute top-3 left-3">
        <img :src="imgUrl" alt="sneakers" class="
            w-full
        ">
        
        <p class = "text-[10px] mt-2">
            {{ title }}
        </p>
        <div class="w-4/5 flex realitive mt-2">
            <div class="flex flex-col">
                <span class="text-[9px] text-slate-400">цена:</span>
                <span class="text-xs">{{ price }}</span>
            </div>
            <img :src="plusPath" @click="addadIt" alt="" class="w-1.5/5 absolute bottom-3 right-3">
        </div>
    </div>
</template>

<style>

</style>
