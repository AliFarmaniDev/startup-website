<script setup>
import Container from '@/layout/Container.vue'
</script>

<template>
  <div class="w-full my-6">
    <Container>
      <div class="w-full flex flex-col sm:flex-row">
        <div class="flex flex-col justify-end gap-3 order-2 mt-4">
          <!--text box-->
          <h2 class="text-wrap text-[20px] font-bold text-[#212529] sm:text-[25px]">
            Lorem ipsum dolor sit amet consectetur.
          </h2>
          <p class="text-wrap text-[#212529c5] text-[15px] font-medium sm:text-[10px]">
            Lorem ipsum dolor sit amet consectetur adipisicing elit. Beatae sit, exercitationem vel
            maxime eos explicabo accusantium reiciendis, aperiam dolore itaque repellat, maiores
            quo. Nisi magni minima doloremque necessitatibus repudiandae. Reprehenderit.
          </p>
          <button
            class="capitalize bg-[#212529] flex justify-center items-center text-[#FFFFFF] w-[170px] h-[48px] sm:w-[160px] sm:h-[40px] rounded-[5px] text-[18px] font-medium"
          >
            learn more
          </button>
        </div>
        <div class="order-1 sm:order-2 flex items-center">
          <!--image box-->
          <img
            src="../assets/images/image2.png"
            alt="a man work with computer"
            class="flex sm:hidden"
          />
          <img
            src="../assets/images/desctop-image2.png"
            alt="a man work with computer"
            class="hidden sm:flex sm:w-[1150px] sm:h-[331px]"
          />
        </div>
      </div>
    </Container>
  </div>
</template>
