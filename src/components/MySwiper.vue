<template>
  <swiper
    :modules="modules"
    :slides-per-view="1"
    :pagination="{ clickable: true }"
    class="pb-12 bg-gradient-to-b from-primary-200/20 to-secondary-/20 rounded-lg"
  >
    <swiper-slide class="grid place-items-center">
      <img src="../assets/images/garri01.png" class="w-2/3 lg:w-[80%] pt-5" alt="groceries, sweetners, cream and floating berries and ice" />
    </swiper-slide>
    <swiper-slide class="grid place-items-center">
      <img src="../assets/images/garri02.png" class="w-2/3 lg:w-[80%] pt-5" alt="groceries, floating berries and ice" />
    </swiper-slide>
    <swiper-slide class="grid place-items-center">
      <img src="../assets/images/akara.png" class="w-2/3 lg:w-[80%] pt-5 rotate-90" alt="akara" />
    </swiper-slide>
    <swiper-slide class="grid place-items-center">
      <img src="../assets/images/kulikuli03.png" class="w-2/3 lg:w-[80%] pt-5" alt="Kuli-kuli" />
    </swiper-slide>
    <swiper-slide class="grid place-items-center h-60">
      <img src="../assets/images/moimoi.png" class="w-[90%]" alt="Moi-Moi" />
    </swiper-slide>
  </swiper>
</template>

<script setup>
// import Swiper core and required modules
import { Pagination } from 'swiper';

// Import Swiper Vue.js components
import { Swiper, SwiperSlide } from 'swiper/vue';

// Import Swiper styles
import 'swiper/css';
import 'swiper/css/pagination';

const modules = [Pagination]

</script>

<style>
  .swiper-pagination-bullet {
    @apply w-3 h-3 bg-white opacity-100
  }
  .swiper-pagination-bullet.swiper-pagination-bullet-active {
    @apply rounded-xl w-6  bg-secondary
  }
  .image_card {
    display: flex;
    margin: 0 auto;
    padding: 1.5rem;
    border-radius: 0.5rem;
    box-shadow: 0 20px 25px -5px rgba(0, 0, 0, 0.1), 0 10px 10px -5px rgba(0, 0, 0, 0.04);
  }
</style>

<!--bg-gradient-to-r from-secondary-500-->