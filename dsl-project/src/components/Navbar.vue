<script setup>
import { ref } from 'vue'
const isMenuOpen = ref(false)
function toggleMenu() {
  isMenuOpen.value = !isMenuOpen.value
}
</script>

<template>
<nav class="bg-white shadow-md">
  <div class="container max-w-7xl px-4 py-2 mx-auto">
    <div class="flex justify-between items-center w-full">
      <!-- Left side: Logo and Text -->
      <div class="flex items-center space-x-4">
        <img src="/src/assets/img/logo.jpg" alt="Logo" class="h-10">
        <div>
          <p class="text-black text-lg lg:text-2xl font-bold">MFU DSL EQUEUE</p>
          <p class="text-black text-sm lg:text-md font-bold">ระบบจองคิว กยศ มหาวิทยาลัยแม่ฟ้าหลวง</p>
        </div>
      </div>
      
      <!-- Right side: Logout Button (hidden on small screens) -->
      <div class="hidden md:block ml-auto">
        <button class="bg-indigo-900 hover:bg-indigo-700 text-white font-bold py-2 px-4 text-sm rounded-3xl">
          ออกจากระบบ <i class="pi pi-sign-out"></i>
        </button>
      </div>

      <!-- Mobile Hamburger Menu Button -->
      <div class="md:hidden">
        <button @click="toggleMenu" class="text-indigo-900 hover:text-indigo-700" aria-label="Toggle menu">
          <i class="pi pi-bars text-xl"></i>
        </button>
      </div>
    </div>
  </div>

  <!-- Mobile Menu -->
  <div v-if="isMenuOpen" class="md:hidden bg-white shadow-md">
    <div class="flex flex-col space-y-4 px-4 py-2">
      <button class="bg-indigo-900 hover:bg-indigo-700 text-white font-bold py-2 px-4 text-sm rounded-3xl">
        ออกจากระบบ <i class="pi pi-sign-out"></i>
      </button>
    </div>
  </div>
</nav>
</template>