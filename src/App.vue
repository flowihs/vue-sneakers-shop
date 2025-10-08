<script setup>
  import Header from "@/components/Header.vue";
  import CardList from "@/components/CardList.vue";

  const items = [];

</script>

<template>
<!--  <Drawer />-->

  <div class="w-4/5 m-auto bg-white rounded-xl shadow-xl  mt-14">
    <Header />
    <div class="p-10">
      <div class="flex justify-between items-center">
        <h2 class="text-3xl font-bold mb-8">Все кроссовки:</h2>
        <div class="flex gap-4">
          <select class="py-2 px-3 border-gray-200 outline-none transition border rounded-md cursor-pointer">
            <option>По названию</option>
            <option>По цене (дешевые)</option>
            <option>По цене (дорогие)</option>
          </select>

          <div class="relative">
            <img
                src="/search.svg"
                class="absolute left-4 top-3"
            >

            <input
                placeholder="Поиск..."
                class="border border-gray-200 rounded-md py-2 pl-11 pr-4 outline-none focus:border-gray-400 transition"
            >
          </div>
        </div>

      </div>

      <CardList :items="items" />
    </div>
  </div>
</template>

