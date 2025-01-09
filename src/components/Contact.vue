<script setup>
import Container from '@/layout/Container.vue'
</script>

<template>
  <div class="w-full">
    <Container>
      <div class="w-full flex sm:gap-10 items-center flex-col sm:flex-row my-5 sm:my-12">
        <div class="flex flex-col order-2 gap-3 justify-end my-5 sm:p-5">
          <!--text box-->
          <h2 class="text-wrap text-[#212529] font-medium text-[18px] sm:font-bold sm:text-[25px]">
            Lorem ipsum dolor sit amet consectetur adipisicing.
          </h2>
          <p class="text-wrap text-[#212529c5] text-[15px] font-medium sm:text-[10px]">
            Lorem ipsum dolor, sit amet consectetur adipisicing elit. Sit officia id repellat eius
            minima facere explicabo itaque vel, aliquam unde. Est nemo cumque labore ea, tempore
            fuga harum nesciunt quo.
          </p>
          <button
            class="capitalize bg-[#212529] flex justify-center items-center text-[#FFFFFF] w-[170px] h-[48px] rounded-[5px] text-[18px] font-medium sm:w-[160px] sm:h-[40px]"
          >
            learn more
          </button>
        </div>
        <div class="order-1">
          <!--image box-->
          <img src="../assets/images/image1.png" alt="pepole worke on pc" class="flex sm:hidden" />
          <img
            src="../assets/images/desctop-image1.png"
            alt="pepole worke on pc"
            class="hidden sm:flex sm:w-[1150px] sm:h-[331px]"
          />
        </div>
      </div>
    </Container>
  </div>
</template>
