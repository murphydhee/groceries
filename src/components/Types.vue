<template>
  <section id="types" class="flex flex-col items-center py-32">
    <h2 class="my-10 text-5xl md:text-6xl font-bold text-white">Types of Groceries</h2>
    <div class="grid grid-cols-1 md:grid-cols-2 place-items-center">
      <div v-for="category of categories" :key="category.title" class="text-white grid place-items-center gap-5 text-center text-justify">
        <div class="bg-gradient-to-b from-primary-200/20 to-secondary-/20 rounded-lg">
          <img :src="category.image" class="lg:w-[100%] pt-5" alt="category1">
        </div>
        <h3 class="text-3xl font-bold">{{ category.title }}</h3>
        <p class="w-3/4">{{ category.desc}}</p>
      </div>
    </div>
  </section>


</template>
<script setup>
import category1 from "../assets/images/whitegarri01.png"
import category2 from "../assets/images/yellowgarri02.png"

const categories = [
  {
    title: 'Silver or Vanilla flavour',
    image: category1,
    desc: 'Lorem ipsum dolor sit amet, consectetur adipiscing elit. Id id consequat, eu faucibus nulla. Ultrices mattis lacus, sed maecenas nascetur.'
  },
  {
    title: 'Gold or Banana flavour',
    image: category2,
    desc: 'Lorem ipsum dolor sit amet, consectetur adipiscing elit. Id id consequat, eu faucibus nulla. Ultrices mattis lacus, sed maecenas nascetur.'
  },
]
</script>