<script setup>
import Container from '@/layout/Container.vue';
</script>

<template>
    <div class="w-full flex flex-col">
        <Container>
            <div class="flex justify-center items-center flex-col gap-3 my-5 sm:my-8">
                <!--text box-->
                <span class="uppercase text-[#74C69D] font-bold tracking-[5px]">partners</span>
                <h2 class="text-[#000000] text-[28px] font-bold">Lorem, ipsum dolor.</h2>
                <p class="text-wrap text-[#000000] text-[18px] font-medium text-center">Lorem ipsum dolor sit amet, consectetur adipisicing elit.</p>
                <span class="text-center text-[#000000] text-[18px] font-medium">Lorem, ipsum.</span>
            </div>
            <div class="flex flex-col sm:flex-row justify-center items-center gap-10 sm:justify-between w-full">
                <!--logos-->
                <img src="../assets/images/google.png" alt="google logo">
                <img src="../assets/images/microsoft.png" alt="">
                <img src="../assets/images/airbnb.png" alt="">
                <img src="../assets/images/spotify.png" alt="">
                <button class="capitalize bg-[#212529] flex justify-center items-center text-[#FFFFFF] w-[170px] h-[48px] rounded-[5px] text-[18px] font-medium sm:hidden">learn more</button>
            </div>
            <div class="flex justify-center items-center my-6">
                <button class="capitalize bg-[#212529] flex justify-center items-center text-[#FFFFFF] w-[170px] h-[48px] rounded-[5px] text-[18px] font-medium">learn more</button>
            </div>
        </Container>
    </div>
</template>