
<script setup>
import { useUserStore} from '@/stores/user'

const userStore = useUserStore()

</script>

<template>
    <div>
      <!-- Navigation -->
      <nav class="p-6 flex items-center justify-between bg-gradient-to-r from-black to-green-600">
        <NuxtLink to="/" class="text-2xl text-white font-bold">NuxD</NuxtLink>
  
        <div class="flex items-center space-x-4">
          <NuxtLink to="/" class="text-xl text-white hover:text-teal-300 font-mono">Home</NuxtLink>
          <NuxtLink to="/browse" class="text-xl text-white hover:text-teal-300 font-mono">Browse</NuxtLink>
        </div>
      </nav>
  
      <!-- Main content -->
      <div>
        <slot />
      </div>
  
      <!-- Footer -->
      <footer class="p-6 bg-gradient-to-r from-black to-green-600">
        <div class="container mx-auto flex flex-col md:flex-row items-center justify-between">
          <p class="text-gray-300 text-center md:text-left">Copyright &copy; 2024 - NuxD</p>
          <div class="flex mt-4 md:mt-0 items-center space-x-4">
            <template v-if="userStore.user.isAuthenticated">
              <NuxtLink to="/myjobs" class="py-2 px-4 bg-green-600 hover:bg-green-500 text-white rounded-lg transition duration-300">My Jobs</NuxtLink>
                <NuxtLink to="/createjob" class="py-2 px-4 bg-green-400 hover:bg-green-300 text-white rounded-lg transition duration-300">Create Jobs</NuxtLink>
                <NuxtLink to="/logout" class="py-2 px-4 bg-red-400 hover:bg-red-300 text-white rounded-lg transition duration-300">Log Out</NuxtLink>
              </template>
              <template v-else>
                <NuxtLink to="/login" class="py-2 px-4 bg-green-600 hover:bg-green-500 text-white rounded-lg transition duration-300">Log In</NuxtLink>
                <NuxtLink to="/signup" class="py-2 px-4 bg-green-400 hover:bg-green-300 text-white rounded-lg transition duration-300">Sign Up</NuxtLink>
            </template>
          </div>
        </div>
      </footer>
    </div>
  </template>