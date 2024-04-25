<template>
    <div class="py-10 px-6 grid gap-3 bg-gradient-to-r from-black to-green-600">
        <h1 class="mb-6 text-2xl text-white">Create Job</h1>

        <form class="space-y-4">
            <div>
                <label class="text-white">Category</label>

                <select class="w-full mt-2 p-4 rounded-xl bg-gray-100">
                    <option value="">Select Category</option>
                    <option value="cat1">Category 1</option>
                    <option value="cat2">Category 2</option>
                </select>
            </div>
            <div>
                <label class="text-white">Title</label>
                <input type="text" class="w-full mt-2 p-4 rounded-xl bg-gray-100">
            </div>
            <div>
                <label class="text-white">Description</label>
                <textarea type="text" class="w-full mt-2 p-4 rounded-xl bg-gray-100"></textarea>
            </div>
            <div>
                <label class="text-white">Salary</label>
                <input type="text" class="w-full mt-2 p-4 rounded-xl bg-gray-100">
            </div>
            <div>
                <label class="text-white">Location</label>
                <input type="text" class="w-full mt-2 p-4 rounded-xl bg-gray-100">
            </div>
            <div>
                <label class="text-white">Company Name</label>
                <input type="text" class="w-full mt-2 p-4 rounded-xl bg-gray-100">
            </div>
            <div>
                <label class="text-white">Company Location</label>
                <input type="text" class="w-full mt-2 p-4 rounded-xl bg-gray-100">
            </div>
            <div>
                <label class="text-white">Company email</label>
                <input type="text" class="w-full mt-2 p-4 rounded-xl bg-gray-100">
            </div>
            
            <button class="py-4 px-6 bg-green-900 text-white rounded-xl">Submit</button>
        </form>
    </div>
</template>