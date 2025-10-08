<script setup>

import CartItem from "@/components/CartItem.vue";
</script>

<template>
  <div class="flex flex-col flex-1 gap-4 justify-between">
    <CartItem imageUrl="/sneakers/sneakers-1.jpg" title="Кроссовки Nike Air Max 270" :price="1205" />
    <CartItem imageUrl="/sneakers/sneakers-1.jpg" title="Кроссовки Nike Air Max 270" :price="1205" />
    <CartItem imageUrl="/sneakers/sneakers-1.jpg" title="Кроссовки Nike Air Max 270" :price="1205" />
    <CartItem imageUrl="/sneakers/sneakers-1.jpg" title="Кроссовки Nike Air Max 270" :price="1205" />
    <CartItem imageUrl="/sneakers/sneakers-1.jpg" title="Кроссовки Nike Air Max 270" :price="1205" />
  </div>
</template>