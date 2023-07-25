<template>
  <section id="types" class="flex flex-col items-center py-32">
    <h2 class="my-10 text-5xl md:text-6xl font-bold text-white">Types of Groceries</h2>
    <div class="grid grid-cols-1 md:grid-cols-2 place-items-center bg-gradient-to-b from-primary-200/30 rounded-lg pb-4">
      <div v-for="category of categories" :key="category.title" class="text-white grid place-items-center gap-5 text-center text-justify">
        <div>
          <img :src="category.image" class="lg:w-[100%] pt-5 inline-block align-baseline" alt="category1">
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
    desc: 'Our Vanilla Groceries starts with premium cassava, just like the classic staple you know and love. But we take it up a notch by infusing it with the smooth, rich essence of vanilla, creating a symphony of taste that\'s both familiar and extraordinary.A delightful marriage with a tantalizing twist of tradition and flavor.'
  },
  {
    title: 'Gold or Banana flavour',
    image: category2,
    desc: 'A delightful symphony of Africa\'s heritage and the exotic allure of ripe bananas. Discover the perfect harmony of tradition and innovation, Each spoonful takes you on a blissful journey to a tropical paradise, leaving you craving more.'
  },
]
</script>