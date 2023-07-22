<template>
  <swiper
    :modules="modules"
    :slides-per-view="1"
    :pagination="{ clickable: true }"
    class="pb-8"
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
</style>