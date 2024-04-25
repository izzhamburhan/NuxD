<template>
    <div class="py-10 px-6 grid md:grid-cols-4 gap-3 bg-gradient-to-r from-black to-green-600">
        <div class="md:col-span-3">
            <h1 class="mb-6 text-3xl text-white">The Title</h1>

            <p class="mb-6 text-white">
                The description of the jobb
            </p>

            <a href="#" class="inline-block mt-6 py-4 px-6 bg-green-900 text-white rounded-xl">Apply</a>
        </div>

        <div class="md:col-span-1 p-6 relative rounded-xl border border-gray-600">
            <div class="absolute inset-0 bg-black opacity-50 rounded-xl"></div> <!-- Semi-transparent overlay -->
            <div class="relative z-10">
                <h3 class="mb-6 text-2xl text-white">Company</h3>
                <p class="text-white">Location</p>

                <hr class="my-6 opacity-30">

                <h3 class="mb-6 text-2xl text-white">Position</h3>
                <p class="text-white mb-2">Position Location</p>
                <p class="text-white">Salary</p>

                <hr class="my-6 opacity-30">

                <p class="text-white">Posted at Dec.1 2024</p>
            </div>
        </div>

    </div>
</template>