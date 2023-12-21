<template>
  <section id="recipes" class="flex flex-col items-center py-32">
    <h2 class="mt-10 mb-28 text-5xl md:text-6xl font-bold text-white">
      Groceries Features
    </h2>
    <div
      class="grid grid-cols-3 lg:grid-cols-3 md:grid-cols-1 xs:grid-cols-1 gap-5 lg:gap-10"
    >
      <div
        v-for="(tot, i) of tots"
        :key="tot.title"
        class="grid place-items-center text-center gap-5 p-8 rounded-md text-white bg-gradient-to-b from-primary-200/20 to-primary-200/10 hover:bg-primary-200"
      >
        <div class="img_margin object-contain md:mx-0 container lg">
          <img :src="tot.image" alt="" />
        </div>
        <h3 class="text-2xl lg:text-4xl font-bold">{{ tot.title }}</h3>
        <p class="w-[90%] md:block">{{ tot.desc }}</p>
      </div>
    </div>
  </section>

  <!--  Honorable mention section-->

  <section
    class="grid grid-flow-col grid-cols-1 md:grid-cols-2 md:gap-10 items-center"
  >
    <div
      class="md:p-10 bg-gradient-to-b from-secondary-/20 to-primary-200/10 rounded-lg"
    >
      <img src="../assets/images/garricookies01.png" alt="Garri Cookies" />
    </div>
    <div class="text-center flex flex-col items-center">
      <h2 class="text-5xl md:text-6xl font-bold text-white">Honorable</h2>
      <div class="flex items-center gap-5">
        <h2 class="text-5xl md:text-6xl font-bold text-white">Mention</h2>
      </div>
      <div>
        <h3 class="text-4xl md:text-4xl font-bold text-secondary pt-3.5">
          Garri Cookies
        </h3>
      </div>
      <p class="mt-8 md:mt-12 text-white text-lg md:text-xl w-full md:w-[80%]">
        These subtly sweet cookies are crisp and delicious. They are made from
        similar ingredients of sweetners & optional floating berries for
        flavour.
      </p>
    </div>
  </section>
</template>

<script setup>
import tots from "../data/features";
</script>

<style scoped>
.img_margin {
  margin: 0 !important;
  display: inline-flex !important;
  justify-content: center;
}
</style>
