<template>
  <section class="hero bg-orange-100 py-[150px] lg:py-[200px] text-center relative overflow-hidden ">
    <div class="container mx-auto px-[30px]">
      <div class="grid grid-cols-12 gap-4 items-center lg:py-[100px]">
        <div class="left-side col-span-5 text-left z-1 relative" data-aos="fade-up ">
          <h1 class="text-4xl font-bold mb-4">
            Pet Shop Terlengkap untuk Kebutuhan Hewan Peliharaan Anda
          </h1>
          <p class="mb-6">Dapatkan diskon spesial untuk pembelian pertama!</p>
            <button class="bg-black text-white px-6 py-2 rounded flex items-center space-x-2">
            <span>Selengkapnya</span>
            <svg class="arrow-animation w-4 h-4" xmlns="http://www.w3.org/2000/svg" fill="none" viewBox="0 0 24 24" stroke="currentColor" stroke-width="2">
              <path stroke-linecap="round" stroke-linejoin="round" d="M9 5l7 7-7 7" />
            </svg>
            </button>
        </div>
        <div class="right-side col-span-7 flex justify-center space-x-4 relative z-0">

          <img :src="bg" alt="Cat 2" class="absolute bottom-[-600px] left-[0] animate-translate-y" />
          <img :src="cat1" alt="Cat 1" class="absolute bottom-[-280px] left-[-20px] lg:bottom-[-700px] md:bottom-[-580px] lg:left-[0px] opacity-50 md:opacity-100" />
          <img :src="cat2" alt="Cat 2" class="absolute lg:bottom-[-700px] md:bottom-[-480px] lg:left-[370px] w-[250px] lg:w-[auto] bottom-[-340px] left-[180px] opacity-50 md:opacity-100" />

            <img :src="ball1" alt="Cat 2" class="absolute lg:top-[-380px] lg:left-[-600px] left-[-160px] top-[-360px] animate-translate-y" />
          <img :src="ball2" alt="Cat 2" class="absolute lg:bottom-[-490px] lg:right-[720px] right-[-290px] bottom-[-250px] animate-translate-y" />
        </div>
      </div>
      <div class="scroll-down-animation absolute bottom-10 left-1/2 transform -translate-x-1/2 text-center text-[#fff]">
        <svg class="mx-auto" xmlns="http://www.w3.org/2000/svg" width="40px" height="40px" viewBox="0 0 24 24" fill="none">
          <path d="M5 15C5 16.8565 5.73754 18.6371 7.05029 19.9498C8.36305 21.2626 10.1435 21.9999 12 21.9999C13.8565 21.9999 15.637 21.2626 16.9498 19.9498C18.2625 18.6371 19 16.8565 19 15V9C19 7.14348 18.2625 5.36305 16.9498 4.05029C15.637 2.73754 13.8565 2 12 2C10.1435 2 8.36305 2.73754 7.05029 4.05029C5.73754 5.36305 5 7.14348 5 9V15Z" stroke="#fff" stroke-width="1.5" stroke-linecap="round" stroke-linejoin="round"/>
          <path d="M12 6V14" stroke="#fff" stroke-width="1.5" stroke-linecap="round" stroke-linejoin="round"/>
          <path d="M15 11L12 14L9 11" stroke="#fff" stroke-width="1.5" stroke-linecap="round" stroke-linejoin="round"/>
        </svg>
        Scroll Down
      </div>

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
      .scroll-down-animation {
        animation: bounce 2s infinite;
      }

      @keyframes bounce {
        0%, 100% {
          transform: translate(-50%, 0);
        }
        50% {
          transform: translate(-50%, 10px);
        }
      }

      .scroll-icon {
        animation: fade 2s infinite;
      }

      @keyframes fade {
        0%, 100% {
          opacity: 1;
        }
        50% {
          opacity: 0.5;
        }
      }
      </style>
    </div>
  </section>
</template>

<script setup>
const cat1 = '/assets/float-hero1.png';
const cat2 = '/assets/float-hero2.png';
const bg = '/assets/float-hero3.png';
const ball1 = '/assets/float-hero4.png';
const ball2 = '/assets/float-hero5.png';
</script>

<style scoped>
.hero {
  background: linear-gradient(135deg, #ffecd2, #fcb69f);
}
@media (max-width: 768px) {
  .col-span-5 {
    grid-column: span 12 / span 12;
  }
}

.right-side {
  position: relative;
  z-index: 0;
}
.left-side {
  position: relative;
  z-index: 1;
}
.animate-translate-y {
  animation: translateY-bounce 2s infinite;
}

@keyframes translateY-bounce {
  0%, 100% {
    transform: translateY(0);
  }
  50% {
    transform: translateY(-10px);
  }
}
</style>
