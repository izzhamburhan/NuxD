<script setup>
const {data: jobs} = await useFetch('http://localhost:8000/api/v1/jobs/newest/')
</script>
<template>
    <div>
         <div class="py-20 px-6 bg-gradient-to-r from-black to-green-600 text-center font-mono font-bold">
             <h1 class="mb-12 text-5xl text-white">Find a job anywhere</h1>
 
             <NuxtLink to="/browse" class="inline-block py-4 px-6 bg-green-800 hover:bg-green-700 text-white rounded-xl">Browse</NuxtLink>
         </div>
 
         <div class="py-10 px-6 bg-gradient-to-r from-black to-green-600">
             <h2 class="mb-8 text-2xl text-center text-white font-mono">Newest Job</h2>
 
             <div class="space-y-4">
                 <Job 
                 v-for="job in jobs" 
                 v-bind:key="job.id"
                 v-bind:job="job"
                 />
             </div>
         </div>
     </div>
 </template>
 