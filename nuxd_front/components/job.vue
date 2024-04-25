<script setup>
const props = defineProps({
    my:{
        type:[Boolean]
    },
    job:{
        type: [Object]
    }
})
</script>

<template>
    <div class="p-6 flex items-center justify-between bg-gray-100 rounded-xl">
                     <div>
                         <h3 class="mb-2 text-xl font-semibold">{{ job.title }}</h3>
                         <p class="text-gray=600" >{{ job.company_name }} </p>
                     </div>
 
                     <div>
                         <p class="mb-2">{{ job.position_location }}</p>
                         <p>{{ job.position_salary }}</p>
                     </div>
 
                     <div>
                         <p>Posted {{ job.created_at_formatted }}</p>
                     </div>
 
                     <div class="space-x-4">
                         <NuxtLink v-bind:to="'/browse/' + job.id" class="py-4 px-6 bg-green-700 hover:bg-green-600 text-white rounded-xl">Details</NuxtLink>
                         <NuxtLink v-bind:to="'/browse/' + job.id" class="py-4 px-6 bg-yellow-500 hover:bg-yellow-600 text-white rounded-xl" v-if="my" >Edit</NuxtLink>
                         <NuxtLink v-bind:to="'/browse/' + job.id" class="py-4 px-6 bg-red-700 hover:bg-red-600 text-white rounded-xl" v-if="my" >Delete</NuxtLink>
                     </div>
                 </div>
</template>