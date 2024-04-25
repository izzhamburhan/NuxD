<template>
    <div class="py-10 px-6 bg-gradient-to-r from-black to-green-600" >
        <div class=" max-w-sm mx-auto md:col-span-1 p-6 relative rounded-xl border border-gray-600">
            <div class=" absolute inset-0 bg-black opacity-50 rounded-xl"></div> <!-- Semi-transparent overlay -->
            <div class="relative z-10">
                <h1 class="mb-6 text-2xl text-white">Log In</h1>

                <form>
                    <input type="email" placeholder="Your email address..." class="w-full mb-4 py-4 px-6 rounded-xl">
                    <input type="password" placeholder="Your password..." class="w-full mb-4 py-4 px-6 rounded-xl">

                    <button class="py-4 px-6 bg-green-900 text-white rounded-xl">Submit</button>
                </form>
            </div>
        </div>

    </div>
</template>