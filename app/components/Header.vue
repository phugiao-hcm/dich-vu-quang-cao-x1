<template>
  <header class="w-full bg-gray-900 text-white py-4 px-6 shadow-md">
    <div class="max-w-screen-xl mx-auto flex items-center justify-between">
      <!-- Logo -->
      <div class="flex items-center gap-2">
        <img src="/images/logo.png" alt="Logo" class="h-10" />
        <span class="text-lg font-semibold text-white hidden md:inline"
          >Phước Hòa Print</span
        >
      </div>

      <!-- Desktop Navigation -->
      <nav
        class="hidden lg:flex items-center gap-6 text-sm font-medium text-gray-300"
      >
        <NuxtLink to="/" class="hover:text-blue-400 transition-colors"
          >ẤN PHẨM F&B</NuxtLink
        >
        <NuxtLink to="/" class="hover:text-blue-400 transition-colors"
          >ẤN PHẨM VĂN PHÒNG</NuxtLink
        >
        <NuxtLink to="/" class="hover:text-blue-400 transition-colors"
          >ẤN PHẨM TIẾP THỊ</NuxtLink
        >
        <NuxtLink to="/" class="hover:text-blue-400 transition-colors"
          >ẤN PHẨM BAO BÌ</NuxtLink
        >
        <NuxtLink to="/" class="hover:text-blue-400 transition-colors"
          >ẤN PHẨM CÁ NHÂN</NuxtLink
        >
      </nav>

      <!-- Hamburger (Mobile only) -->
      <button
        @click="menuOpen = !menuOpen"
        class="lg:hidden ml-4 text-white focus:outline-none"
      >
        <svg
          class="w-6 h-6"
          fill="none"
          stroke="currentColor"
          stroke-width="2"
          viewBox="0 0 24 24"
        >
          <path
            stroke-linecap="round"
            stroke-linejoin="round"
            d="M4 6h16M4 12h16M4 18h16"
          />
        </svg>
      </button>
    </div>

    <!-- Mobile Menu -->
    <div v-if="menuOpen" class="lg:hidden mt-4 px-6">
      <div class="flex flex-col space-y-3 text-sm font-medium text-gray-300">
        <NuxtLink to="/" class="hover:text-blue-400 transition-colors"
          >ẤN PHẨM F&B</NuxtLink
        >
        <NuxtLink to="/" class="hover:text-blue-400 transition-colors"
          >ẤN PHẨM VĂN PHÒNG</NuxtLink
        >
        <NuxtLink to="/" class="hover:text-blue-400 transition-colors"
          >ẤN PHẨM TIẾP THỊ</NuxtLink
        >
        <NuxtLink to="/" class="hover:text-blue-400 transition-colors"
          >ẤN PHẨM BAO BÌ</NuxtLink
        >
        <NuxtLink to="/" class="hover:text-blue-400 transition-colors"
          >ẤN PHẨM CÁ NHÂN</NuxtLink
        >
      </div>
    </div>
  </header>
</template>

<script setup>
import { ref } from "vue";
const menuOpen = ref(false);
</script>
