<script setup>
import { RouterLink } from 'vue-router';
//impoting components
import Container from '@/layout/Container.vue';
import Navigation from './Navigation.vue';
</script>

<template>
    <header class="w-full bg-[#74C69D]">
        <Container class="py-3 sm:py-4 md:py-5 flex justify-between items-center">
            <div class="flex items-center">
                <!--this is logo section-->
                <RouterLink to="/">
                    <img src="../assets/images/Frame 4.png" alt="site logo" class="w-[129px] h-[38px] sm:w-[187px] sm:h-[50px]">
                </RouterLink>
            </div>
            <div class="flex items-center">
                <!--menu section-->
                <Navigation/>
            </div>
        </Container>
    </header>
</template>