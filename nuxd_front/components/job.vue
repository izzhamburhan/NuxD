<script setup>
const props = defineProps({
    my:{
        type:[Boolean]
    }
})
</script>

<template>
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
 
                     <div class="space-x-4">
                        <NuxtLink to="/browse/1" class="py-4 px-6 bg-green-700 hover:bg-green-600 text-white rounded-xl">Details</NuxtLink>
                         <NuxtLink to="/browse/1" class="py-4 px-6 bg-yellow-500 hover:bg-yellow-600 text-white rounded-xl" v-if="my" >Edit</NuxtLink>
                         <NuxtLink to="/browse/1" class="py-4 px-6 bg-red-700 hover:bg-red-600 text-white rounded-xl" v-if="my" >Delete</NuxtLink>
                     </div>
                 </div>
</template>