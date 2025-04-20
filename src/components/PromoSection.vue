<template>
  <section class="py-[80px] px-4 bg-[#F8F9FA]">
    <div class="container mx-auto px-[30px]">
      <div class="grid md:grid-cols-2 lg:grid-cols-3 gap-[24px]">
      <div v-for="(n, index) in 3" :key="n" class="text-center">
        <img 
          class="mask mask-circle w-full h-auto"
          data-aos="fade-left"
          :data-aos-delay="index * 200"
          :data-aos-duration="1000"
          :data-aos-easing="'ease-in-out'"
          :data-aos-offset="100" 
          width="300" 
          height="300" 
          :src="`/assets/banner${n}.jpg`" 
          alt="Profile image" 
        />
      </div>
    </div>
    </div>
  </section>
</template>
