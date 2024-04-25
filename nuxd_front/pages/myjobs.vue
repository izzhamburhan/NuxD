

<template>
    <div class="py-10 px-6 grid bg-gradient-to-r from-black to-green-600">
        <h1 class="mb-6 text-2xl text-white">My Job</h1>

            <div class="space-y-4">
                    <Job :my="true"/>
                    <Job :my="true"/>
                    <Job :my="true"/>
            </div>
    </div>
</template>