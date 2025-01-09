<script setup>
import { RouterLink } from 'vue-router'
import { ref, computed } from 'vue'
</script>

<template>
  <div class="hidden sm:flex items-center">
    <nav class="flex gap-4 items-cente text-[#FFFFFF] font-medium text-[15px]">
      <RouterLink to="/">Home</RouterLink>
      <RouterLink to="/portfolio">Portfolio</RouterLink>
      <RouterLink to="/our-service">Services</RouterLink>
      <RouterLink to="/contact">Contact</RouterLink>
    </nav>
  </div>
</template>
