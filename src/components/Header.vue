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
          <svg
            xmlns="http://www.w3.org/2000/svg"
            class="h-6 w-6"
            fill="none"
            viewBox="0 0 24 24"
            stroke="currentColor"
          >
            <path
              stroke-linecap="round"
              stroke-linejoin="round"
              stroke-width="2"
              d="M4 6h16M4 12h16m-7 6h7"
            />
          </svg>
        </button>
      </div>
    </Container>
    <!-- mobile dropdown menu -->
    <div v-if="isDropdownOpen" class="md:hidden bg-[#74C69D]">
      <ul class="flex flex-col space-y-2 p-4">
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