<template>
  <section class="py-[80px] px-4">
    <div class="container mx-auto" data-aos="fade-up">
      <h2 class="text-2xl font-bold text-center mb-6">Best Seller</h2>
      <div class="grid md:grid-cols-3 lg:grid-cols-4 gap-4">
        <div v-for="n in 8" :key="n" class="bg-white shadow rounded pb-4 text-center">
            <img :src="`/assets/prod${Math.floor(Math.random() * 3) + 1}.jpg`" class="mb-2 mx-auto w-full rounded rounded-b-none" />
          <h3 class="font-semibold">Premium Cat Food</h3>
          <p class="text-sm">Rp. 99,000</p>
        </div>
      </div>
      <div class="text-center mt-6" data-aos="fade-up" data-aos-delay="300" data-aos-anchor-placement="top-bottom">
        <button class="bg-black text-white px-6 py-2 rounded flex items-center space-x-2 mx-auto">
        <span>Selengkapnya</span>
          <svg class="arrow-animation w-4 h-4" xmlns="http://www.w3.org/2000/svg" fill="none" viewBox="0 0 24 24" stroke="currentColor" stroke-width="2">
        <path stroke-linecap="round" stroke-linejoin="round" d="M9 5l7 7-7 7" />
          </svg>
          </button>
      </div>
    </div>
  </section>
</template>

<style scoped>
.arrow-animation {
  animation: move-right 1s infinite;
  }

  @keyframes move-right {
  0%, 100% {
    transform: translateX(0);
  }
  50% {
    transform: translateX(5px);
  }
  }
</style>