<template>
  <section class="hero bg-orange-100 py-[200px] text-center relative overflow-hidden">
    <div class="container mx-auto px-[30px]">
      <div class="grid grid-cols-12 gap-4 items-center py-[100px]">
        <div class="left-side col-span-5 text-left z-1" data-aos="fade-up">
          <h1 class="text-3xl font-bold mb-4">
            Pet Shop Terlengkap untuk Kebutuhan Hewan Peliharaan Anda
          </h1>
          <p class="mb-6">Dapatkan diskon spesial untuk pembelian pertama!</p>
          <button class="bg-black text-white px-6 py-2 rounded">Selengkapnya</button>
        </div>
        <div class="right-side col-span-7 flex justify-center space-x-4 relative">

          <img :src="bg" alt="Cat 2" class="absolute bottom-[-600px] left-[0]" />
          <img :src="cat1" alt="Cat 1" class="absolute bottom-[-700px] left-[0px]" />
          <img :src="cat2" alt="Cat 2" class="absolute bottom-[-700px] left-[370px]" />
          <img :src="ball1" alt="Cat 2" class="absolute top-[-380px] left-[-460px]" />
          <img :src="ball2" alt="Cat 2" class="absolute bottom-[-490px] left-[-460px]" />
        </div>
      </div>
      
    </div>
  </section>
</template>

<script setup>
const cat1 = '/src/assets/float-hero1.png';
const cat2 = '/src/assets/float-hero2.png';
const bg = '/src/assets/float-hero3.png';
const ball1 = '/src/assets/float-hero4.png';
const ball2 = '/src/assets/float-hero5.png';
</script>

<style scoped>
.hero {
  background: linear-gradient(135deg, #ffecd2, #fcb69f);
}
</style>
