<template>
  <div class="container overflow-x-hidden">
    <Navbar/>
    <Home class="pt-7"/>
    <Category/>
    <Recipes/>
    <Subscribe/>
    <Footer/>
  </div>
</template>

<script setup>
import Navbar from './components/Navbar.vue';
import Home from './components/Home.vue';
import Category from './components/Types.vue';
import Recipes from './components/Recipes.vue';
import Subscribe from './components/Subscribe.vue';
import Footer from './components/Footer.vue';
</script>
