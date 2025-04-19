<template>
  <section class="hero bg-orange-100 py-[200px] text-center relative">
    <div class="container mx-auto">
      <div class="grid grid-cols-12 gap-4 items-center">
        <div class="left-side col-span-5 text-left">
        <h1 class="text-3xl font-bold mb-4">
          Pet Shop Terlengkap untuk Kebutuhan Hewan Peliharaan Anda
        </h1>
        <p class="mb-6">Dapatkan diskon spesial untuk pembelian pertama!</p>
        <button class="bg-black text-white px-6 py-2 rounded">Selengkapnya</button>
        </div>
        <div class="right-side col-span-7 flex justify-center space-x-4">
        <img :src="cat1" alt="Cat 1" class="w-32 h-32 rounded-full" />
        <img :src="cat2" alt="Cat 2" class="w-32 h-32 rounded-full" />
        <img :src="cat3" alt="Cat 3" class="w-32 h-32 rounded-full" />
        </div>
      </div>
    </div>
  </section>
</template>

<script setup>
const cat1 = 'https://placehold.it/300x300';
const cat2 = 'https://placehold.it/300x300';
const cat3 = 'https://placehold.it/300x300';
</script>

<style scoped>
.hero {
  background: linear-gradient(135deg, #ffecd2, #fcb69f);
}
</style>
