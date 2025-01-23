<script setup>
  import { ref } from 'vue'
  import Navbar from '@/components/Navbar.vue';
 import ReviewStar from '@/components/ReviewStar.vue';
 import ReviewForm from '@/components/ReviewForm.vue';
  
  </script>

<template>
    <Navbar/>
    <div class="min-h-screen flex items-center justify-center bg-gray-100">
        <ReviewForm/>
    </div>
  </template>

  