<script setup>
import { ref } from 'vue'

let counter = ref(0)

setInterval(() => {
    counter.value++
}, 1000)
</script>

<template>
    <div>
        <header class="text-gray-400 bg-gray-900 body-font">
            <div class="container mx-auto flex flex-wrap p-5 flex-col md:flex-row items-center">
                <a class="flex title-font font-medium items-center text-white mb-4 md:mb-0">
                    <svg class="w-10 h-10 text-white p-2 bg-indigo-500 rounded-full" fill="none" stroke="currentColor" stroke-linecap="round"
                         stroke-linejoin="round" stroke-width="2"
                         viewBox="0 0 24 24" xmlns="http://www.w3.org/2000/svg">
                        <path d="M12 2L2 7l10 5 10-5-10-5zM2 17l10 5 10-5M2 12l10 5 10-5"></path>
                    </svg>
                    <span class="ml-3 text-xl">DeSimple</span>
                </a>
                <nav class="md:ml-auto flex flex-wrap items-center text-base justify-center">
                    <a class="mr-5 hover:text-white">First Link</a>
                    <a class="mr-5 hover:text-white">Second Link</a>
                    <a class="mr-5 hover:text-white">Third Link</a>
                    <a class="mr-5 hover:text-white">Fourth Link</a>
                </nav>
            </div>
        </header>

        <!--        <header v-if="$route.meta.title" class="bg-white shadow">-->
        <!--            <div class="px-4 py-6 mx-auto max-w-7xl sm:px-6 lg:px-8">-->
        <!--                <h1-->
        <!--                    class="text-3xl font-bold leading-tight text-gray-900"-->
        <!--                    @click="counter = 0"-->
        <!--                >-->
        <!--                    {{ $route.meta.title }} / {{ counter }}-->
        <!--                </h1>-->
        <!--            </div>-->
        <!--        </header>-->
        <main>
            <router-view />
        </main>
    </div>
</template>
