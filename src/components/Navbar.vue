<template>
  <header class="py-2 md:py-1 bg-white flex items-center px-7 justify-between relative shadow-sm">
    <!-- Mobile Menu Button -->
    <button
      class="w-8 flex gap-1 p-2 flex-col sm:hidden outline outline-white rounded bg-[#215DFF] dark:outline dark:outline-white"
      @click="mobileMenuActive = !mobileMenuActive"
    >
      <span class="block w-full h-[2px] bg-white dark:bg-white"></span>
      <span class="block w-full h-[2px] bg-white"></span>
      <span class="block w-full h-[2px] bg-white"></span>
    </button>

    <!-- Logo and Menu -->
    <div class="flex items-center justify-center gap-2">
      <img
        src="/src/assets/purdiacapital.svg"
        class="w-auto h-5"
      />
    </div>
    <ul
  :class="[
    'flex-col  text-md font-semibold text-black-900 gap-1 mr-0 lg:mr-[250px] justify-center items-center bg-white p-4 sm:flex-row absolute top-full left-0 sm:static sm:flex',
    mobileMenuActive ? 'flex shadow-md w-full h-[200px] pl-[30px]' : 'hidden',
    'sm:shadow-none'
  ]"
  class="sm:flex gap-3"
>
<p class="block text-blue-500 font-semibold lg:inline bg-gray-100 px-3 py-2 rounded-lg">Dashboard</p>

  <a href="#" class="block text-gray-600 hover:text-gray-800 lg:inline">Partner</a>
  <div class="flex items-center space-x-2 block lg:inline">
    <a href="#" class="text-gray-600 hover:text-gray-800">Desk Performance</a>
    <span class="bg-red-100 text-red-500 text-xs font-medium px-2 py-0.5 rounded">Beta</span>
  </div>
</ul>
    

    <!-- Profile and Notifications -->
    <div class="flex items-center gap-3">
      <svg class="h-6 w-6 text-white" fill="none"
        viewBox="0 0 24 24"
        stroke-width="1.5"
        stroke="currentColor"
        aria-hidden="true"
      >
        <path
          stroke-linecap="round"
          stroke-linejoin="round"
          d="M14.857 17.082a23.848 23.848 0 005.454-1.31A8.967 8.967 0 0118 9.75v-.7V9A6 6 0 006 9v.75a8.967 8.967 0 01-2.312 6.022c1.733.64 3.56 1.085 5.455 1.31m5.714 0a24.255 24.255 0 01-5.714 0m5.714 0a3 3 0 11-5.714 0"
        />
      </svg>

      <!-- Profile Dropdown -->
      <div class="relative flex gap-3 items-center justify-center">
        <span class="text-sm">Jonas</span>
          <img class="w-10 h-10 rounded-full ring-white ring-2 ring-offset-2 ring-offset-gray-700"
            src="/src/assets/profile.png"/>
      </div>
    </div>
  </header>
</template>

<script>
import { ref } from "vue";

export default {
  name: "Navbarnew",
  setup() {
    const mobileMenuActive = ref(false); // Default to closed menu
    return {
      mobileMenuActive,
    };
  },
};
</script>

<style scoped>
/* Add any additional custom styles if needed */
</style>

