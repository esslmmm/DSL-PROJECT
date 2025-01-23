<script setup>
  import { ref } from 'vue'

//   const selectedOption = ref(null);
// const options = ref([
//   { id: 'success', label: 'ได้รับ' },
//   { id: 'no-success', label: 'ไม่ได้รับ' },
// ]);
// const achievedGoal = ref(false);
// const contentQuality = ref(false);
// const clarity = ref(false);

// function submit() {
//   const response = {
//     success: selectedOption.value === 'success',
//     details: {
//       achievedGoal: achievedGoal.value,
//       contentQuality: contentQuality.value,
//       clarity: clarity.value,
//     },
//   };
//   console.log(response);
//   // You can also emit the response data to a parent component
// }

const helpReceived = null

  
  const handleSubmit = () => {
    console.log('Submitted rating:', rating.value)
    // Add your submission logic here
  }
  </script>
  
  <style scoped>
  
  /* Optional: Add additional button shadow effects */
  button {
    transition: transform 0.2s ease, background-color 0.3s ease;
  }
  </style>

<template>

        <div class="flex flex-col items-center p-28 max-w-sm mx-auto bg-white rounded-lg shadow-lg">
      <!-- Service Icon -->
      <div class="bg-gray-100 p-4 rounded-full mb-6">
        <div class="w-16 h-16 bg-gray-300 rounded-full flex items-center justify-center">
          <svg
            class="w-10 h-10 text-gray-600"
            viewBox="0 0 24 24"
            fill="none"
            stroke="currentColor"
          >
            <path
              stroke-linecap="round"
              stroke-linejoin="round"
              stroke-width="2"
              d="M16 7a4 4 0 11-8 0 4 4 0 018 0zM12 14a7 7 0 00-7 7h14a7 7 0 00-7-7z"
            />
          </svg>
        </div>


        
      </div>



  
      <!-- Submit Button -->
      <button
        @click="handleSubmit"
        class="w-full bg-gradient-to-r from-indigo-600 via-indigo-800 to-indigo-900 text-white py-3 rounded-md shadow-lg hover:scale-105 hover:from-indigo-700 hover:to-indigo-800 transition-all duration-300 ease-in-out transform"
      >
        NEXT
      </button>
    </div>

  </template>

  