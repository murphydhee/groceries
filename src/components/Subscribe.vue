<template>
  <div class="relative my-32 bg-gradient-to-b from-primary-200/30 to-primary-100/10 pb-10 md:pb-32 rounded-lg -mx-5">
    <div class="p-10 ">
      <div class="flex items-center justify-between">
        <div>
          <h2 class="text-4xl sm:text-5xl md:text-6xl font-bold text-white mb-4 mt-5 md:mt-0">Subscribe</h2>
          <p class="text-base md:text-lg text-white md:w-full">Subscribe to our newsletters and stay update!</p>
        </div>
      </div>
      <form action="#" class="mt-14 w-full">
        <div class="h-16 md:h-20 w-full md:w-1/2 flex items-center">
          <input 
            class="h-full flex-grow rounded-l-lg px-3 md:px-6 text-sm md:text-lg" 
            type="text" 
            placeholder="Enter your email address"
          />
          <button class="h-full px-3 lg:px-6 text-sm md:text-base text-white font-bold bg-secondary rounded-r-lg hover:bg-primary-200">SUBSCRIBE</button>
        </div>
      </form>
    </div>
    <div class="absolute right-10 bottom-10 w-1/3 md:block xs: hidden">
      <img src="../assets/images/kulikuli02.png" alt="">
    </div>
  </div>
</template>