<template>
    <div class="flex justify-between items-center py-4 px-6 sticky top-0 z-30 border-b bg-white">
      <div class="flex items-center space-x-2">
        <img src="/images/LOGO.svg" alt="logo" class="">
       
      </div>
  
      <!-- Links for desktop screens -->
      <div class="hidden lg:flex justify-center items-center gap-8">
        <div class="flex space-x-6 text-black font-semibold">
          <a href="#" class="hover:text-gray-400">Home</a>
          <a href="#about" class="hover:text-gray-400">About</a>
          <a href="#contact" class="hover:text-gray-400">Contact</a>
          <a href="#pricing" class="hover:text-gray-400">Pricing</a>
        </div>
        <button class="bg-primary hover:bg-blue-800 text-white px-4 py-2 rounded">
          Login/Signup
        </button>
      </div>
  
      <!-- Burger menu button for mobile and tablet screens -->
      <button
        class="lg:hidden block text-primary focus:outline-none"
        @click="toggleSidebar"
      >
        <svg
          class="w-8 h-8"
          fill="none"
          stroke="currentColor"
          viewBox="0 0 24 24"
          xmlns="http://www.w3.org/2000/svg"
        >
          <path
            stroke-linecap="round"
            stroke-linejoin="round"
            stroke-width="2"
            d="M4 6h16M4 12h16m-7 6h7"
          ></path>
        </svg>
      </button>
  
      <!-- Sidebar for mobile screens -->
      <div
        class="fixed top-0 z-10 right-0 h-full w-64 bg-white shadow-lg transform transition-transform duration-300"
        :class="{'translate-x-full': !sidebarOpen, 'translate-x-0': sidebarOpen}"
      >
        <div class="flex justify-between items-center py-4 px-6 bg-primary text-white">
          <h1 class="text-xl font-bold">Menu</h1>
          <button class="focus:outline-none" @click="toggleSidebar">
            <svg
              class="w-6 h-6"
              fill="none"
              stroke="currentColor"
              viewBox="0 0 24 24"
              xmlns="http://www.w3.org/2000/svg"
            >
              <path
                stroke-linecap="round"
                stroke-linejoin="round"
                stroke-width="2"
                d="M6 18L18 6M6 6l12 12"
              ></path>
            </svg>
          </button>
        </div>
        <div class="flex flex-col space-y-4 px-6 mt-4 text-primary">
          <a href="#" class="hover:text-gray-400">Home</a>
          <a href="#about" class="hover:text-gray-400">About</a>
          <a href="#contact" class="hover:text-gray-400">Contact</a>
          <a href="#pricing" class="hover:text-gray-400">Pricing</a>
          <button class="bg-primary hover:bg-blue-800 text-white px-4 py-2 rounded">
            Login/Signup
          </button>
        </div>
      </div>
    </div>
  </template>
  
  <script setup>
  import { ref } from 'vue';
  
  // Sidebar open state
  const sidebarOpen = ref(false);
  
  // Toggle sidebar
  const toggleSidebar = () => {
    sidebarOpen.value = !sidebarOpen.value;
  };
  </script>
  
  <style scoped>
  /* Optional: Add custom styles if needed */
  </style>
  