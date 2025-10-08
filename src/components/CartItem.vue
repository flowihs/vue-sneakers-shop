<script setup>
  defineProps({
    imageUrl: String,
    title: String,
    price: Number,
  })
</script>

<template>
  <div class="flex  items-center border border-slate-200 p-4 rounded-xl gap-4">
    <img class="w-16 h-16" :src="imageUrl" alt="Sneakers">

    <div class="flex flex-col ">
      <p>{{ title }}</p>
      <div class="flex justify-between mt-2">
        <b>{{ price }} руб.</b>
        <img src="/close.svg" class="cursor-pointer opacity-40 hover:opacity-100 transition">
      </div>
    </div>
  </div>
</template>