<script setup>
import { ref } from 'vue'
import { RouterLink } from 'vue-router'
// importing components
import Container from '@/layout/Container.vue'
import Navigation from './Navigation.vue'

// reactive property to manage dropdown state
const isDropdownOpen = ref(false)

const toggleDropdown = () => {
  isDropdownOpen.value = !isDropdownOpen.value
}
</script>

<template>
  <header class="w-full bg-[#74C69D]">
    <Container class="py-3 sm:py-4 md:py-5 flex justify-between items-center">
      <div class="flex items-center">
        <!-- this is logo section -->
        <RouterLink to="/">
          <img
            src="../assets/images/Frame 4.png"
            alt="site logo"
            class="w-[129px] h-[38px] sm:w-[187px] sm:h-[50px]"
          />
        </RouterLink>
      </div>
      <div class="flex items-center">
        <!-- menu section -->
        <Navigation class="hidden md:block" />
        <!-- mobile menu button -->
        <button @click="toggleDropdown" class="md:hidden">
          <img src="../assets/icons/mobile.png" alt="mobile menu" />
        </button>
      </div>
    </Container>
    <!-- mobile dropdown menu -->
    <div v-if="isDropdownOpen" class="md:hidden bg-[#74C69D]">
      <ul class="flex flex-col space-y-2 p-4 text-[#FFFFFF] font-medium">
        <li>
          <RouterLink to="/" @click="toggleDropdown">Home</RouterLink>
        </li>
        <li>
          <RouterLink to="/about" @click="toggleDropdown">About</RouterLink>
        </li>
        <li>
          <RouterLink to="/services" @click="toggleDropdown">Services</RouterLink>
        </li>
        <li>
          <RouterLink to="/contact" @click="toggleDropdown">Contact</RouterLink>
        </li>
      </ul>
    </div>
  </header>
</template>
