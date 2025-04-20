<template>
  <section class="py-[80px] px-4 bg-[#F8F9FA]">
    <div class="container mx-auto px-[30px]"" 
          data-aos="fade-in">
      <div class="grid md:grid-cols-2 lg:grid-cols-3 gap-[24px]">
      <div v-for="n in 3" :key="n" class="text-center">
        <img 
          class="mask mask-circle w-full h-auto animate__animated animate__fadeInUp" 
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
