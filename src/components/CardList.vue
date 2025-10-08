<script setup lang="ts">
  import Card from "@/components/Card.vue";

  defineProps({
    items: Array,
  })

  const onClickAdd = () => {
    alert("fsdfds")
  }
</script>

<template>
  <div class="grid grid-cols-4 gap-5">

    <Card
        v-for="item in items"
        :key="item.id"
        :imageUrl="item.imageUrl"
        :title="item.title"
        :price="item.price"
        :isFavorite="true"
        :isAdded="true"
        :onClickAdd="onClickAdd"
    />

  </div>
</template>