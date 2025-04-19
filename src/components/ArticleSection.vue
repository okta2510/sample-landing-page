<template>
  <section class="py-[80px] px-4 ">
    <div class="container mx-auto" data-aos="fade-up">
      <h2 class="text-2xl font-bold text-center mb-6">Artikel & Tips</h2>
      <div class="grid md:grid-cols-3 gap-4">
        <div v-for="n in 3" :key="n" class="bg-white rounded-lg p-4">
          <img :src="`/src/assets/artikel${n}.jpg`"" class="mb-3 w-full" />
          <h3 class="font-semibold mb-1">Judul Artikel {{ n }}</h3>
          <p class="text-xs text-gray-600">24 May 2024</p>
        </div>
      </div>
    </div>
  </section>
</template>
