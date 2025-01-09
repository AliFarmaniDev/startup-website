<script setup>
import Container from '@/layout/Container.vue'
</script>

<template>
  <div class="bg-[#74C69D] w-full h-[542px] sm:h-[342px]">
    <Container>
      <div class="flex flex-col sm:flex-row items-center gap-4 py-3 sm:py-5">
        <div class="flex flex-col gap-2 sm:gap-3 order-2">
          <!--text box-->
          <span class="uppercase text-white tracking-[5px]">welcome</span>
          <h2 class="flex text-wrap text-[#FFFFFF] font-bold text-[25px]">
            Lorem ipsum dolor sit amet consectetur.
          </h2>
          <p class="text-[#FFFFFF] text-wrap font-thin">
            Lorem ipsum dolor, sit amet consectetur adipisicing elit. Rerum non fugit soluta ipsa
            illum reprehenderit nostrum ex porro autem odio. Quam, consequatur! Nam, facilis odio
            delectus modi commodi ea voluptas.
          </p>
          <button
            class="capitalize w-[170px] h-[48px] bg-[#FFFFFF] rounded-[5px] text-[18px] font-medium"
          >
            explor
          </button>
        </div>
        <div class="order-1 sm:order-2">
          <!--image box-->
          <img src="../assets/images/mobile-baner.png" alt="baner image" class="flex sm:hidden" />
          <img
            src="../assets/images/desctop.png"
            alt="main banner image"
            class="hidden sm:flex w-[1054px] h-[288px]"
          />
        </div>
      </div>
    </Container>
  </div>
</template>
