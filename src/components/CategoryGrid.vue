<template>
  <section class="py-[50px] px-4">
    <div class="container mx-auto">
      <h2 class="text-2xl font-bold text-center mb-6">Kategori Produk</h2>
      <div class="grid md:grid-cols-2 lg:grid-cols-4 gap-4">
        <div 
          v-for="(cat, i) in categories" 
          :key="i" 
          class="text-center" 
          :data-aos="'flip-up'" 
          :data-aos-delay="i * 100"
        >
          <img :src="cat.image" class="rounded-lg mb-2 w-full" />
          <p>{{ cat.title }}</p>
        </div>
      </div>
    </div>
  </section>
</template>

<script setup>
const categories = [
  { title: 'Makanan Hewan', image: '/assets/cat1.jpg'},
  { title: 'Aksesoris', image: '/assets/cat2.jpg'},
  { title: 'Perawatan', image: '/assets/cat3.jpg'},
  { title: 'Kesehatan', image: '/assets/cat4.jpg'},
];
</script>
