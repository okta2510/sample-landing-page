<template>
  <section class="py-[80px] px-4">
    <div class="container mx-auto" data-aos="fade-up">
      <h2 class="text-2xl font-bold text-center mb-6">Best Seller</h2>
      <div class="grid md:grid-cols-3 lg:grid-cols-4 gap-4">
        <div v-for="n in 8" :key="n" class="bg-white shadow rounded p-4 text-center">
            <img :src="`/src/assets/prod${Math.floor(Math.random() * 3) + 1}.jpg`" class="mb-2 mx-auto w-full" />
          <h3 class="font-semibold">Premium Cat Food</h3>
          <p class="text-sm">Rp. 99,000</p>
        </div>
      </div>
      <div class="text-center mt-6" data-aos="fade-up" data-aos-delay="180">
        <button class="bg-black text-white px-6 py-2 rounded">Lihat Semua</button>
      </div>
    </div>
  </section>
</template>
