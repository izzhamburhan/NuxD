<!-- index.vue -->
<template>
    <div>
         <div class="py-20 px-6 bg-gradient-to-r from-black to-green-600 text-center font-mono font-bold">
             <h1 class="mb-12 text-5xl text-white">Find a job anywhere</h1>
 
             <NuxtLink to="/browse" class="inline-block py-4 px-6 bg-green-800 hover:bg-green-700 text-white rounded-xl">Browse</NuxtLink>
         </div>
 
         <div class="py-10 px-6 bg-gradient-to-r from-black to-green-600">
             <h2 class="mb-8 text-2xl text-center text-white font-mono">Newest Job</h2>
 
             <div class="space-y-4">
                 <div class="p-6 flex items-center justify-between bg-gray-100 rounded-xl">
                     <div>
                         <h3 class="mb-2 text-xl font-semibold">The Job Position</h3>
                         <p class="text-gray=600">The Company Name</p>
                     </div>
 
                     <div>
                         <p class="mb-2">WorldWide</p>
                         <p>RM30-50k</p>
                     </div>
 
                     <div>
                         <p>Posted Dec. 1 2022</p>
                     </div>
 
                     <div>
                         <NuxtLink to="/browse/1" class="py-4 px-6 bg-green-700 hover:bg-green-600 text-white rounded-xl">Details</NuxtLink>
                     </div>
                 </div>
 
                 <div class="space-y-4">
                     <div class="p-6 flex items-center justify-between bg-gray-100 rounded-xl">
                         <div>
                             <h3 class="mb-2 text-xl font-semibold">The Job Position</h3>
                             <p class="text-gray=600">The Company Name</p>
                         </div>
 
                         <div>
                             <p class="mb-2">WorldWide</p>
                             <p>RM30-50k</p>
                         </div>
 
                         <div>
                             <p>Posted Dec. 1 2022</p>
                         </div>
 
                         <div>
                             <NuxtLink to="/browse/1" class="py-4 px-6 bg-green-700 hover:bg-green-600 text-white rounded-xl">Details</NuxtLink>
                         </div>
                     </div>
                 </div>
             </div>
         </div>
     </div>
 </template>
 