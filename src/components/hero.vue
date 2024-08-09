<script setup>
const links = [
    {
        name: 'Home',
        url: '#',
        active: true
    },
    {
        name: 'App',
        url: '#'
    },
    {
        name: 'Freatures',
        url: '#'
    },
    {
        name: 'Testimonials',
        url: '#'
    },
    
]

</script>

<template>
    <header class="sticky top-0 shadow shadow-indigo-50/20 z-10 bg-white dark:bg-indigo-900">
        <nav class="container flex justify-between items-center">
            <div class="flex items-center gap-32">
                <a href="#" class=" text-2xl font-bold">Tonality</a>


                <div class="flex items-center text-xl gap-2">
                    <a href="#"
                     class="px-4 py-4 hover:text-indigo-900 dark:hover:text-indigo-50" 
                     v-for="(link, index) in links" :key="index"
                    :class="{' text-indigo-900 dark:text-indigo-500 font-bold': link.active }">
                        {{ link.name }}

                    </a>

                </div>
            </div>

            <a href="#" class="flex items-center text-indigo-900 font-bold px-7 py-4">
                <span>
                    Get Started
                </span>
                <svg xmlns="http://www.w3.org/2000/svg" viewBox="0 0 24 24" class=" w-10 text-indigo-900 fill-current">
                    <path d="M4,11V13H16L10.5,18.5L11.92,19.92L19.84,12L11.92,4.08L10.5,5.5L16,11H4Z" />
                </svg>



            </a>
        </nav>
    </header>


    <section class="relative py-10">

        <div class="container grid grid-cols-2 gap-7">
            <div class="py-20 space-y-20">
                <h1 class=" text-7xl">
                    You bring the vision, <br>
                    we bring the music
                </h1>
                <p class="text-2xl">
                    With Tonality, you can create music that is as unique as you are. Our tools are designed to help you
                </p>

                <div class=" flex items-center gap-4 text-white">
                    <button
                        class="flex justify-between items-center bg-blue-500 px-4 py-2 rounded-xl text-white gap-2 ">
                        <svg xmlns="http://www.w3.org/2000/svg" viewBox="0 0 24 24" class="w-10 fill-current">
                            <path
                                d="M3,20.5V3.5C3,2.91 3.34,2.39 3.84,2.15L13.69,12L3.84,21.85C3.34,21.6 3,21.09 3,20.5M16.81,15.12L6.05,21.34L14.54,12.85L16.81,15.12M20.16,10.81C20.5,11.08 20.75,11.5 20.75,12C20.75,12.5 20.53,12.9 20.18,13.18L17.89,14.5L15.39,12L17.89,9.5L20.16,10.81M6.05,2.66L16.81,8.88L14.54,11.15L6.05,2.66Z" />
                        </svg>
                        <span class="flex flex-col justify-start text-left">
                            <span class=" uppercase text-xs">Get in on </span>
                            <span class=" text-2xl">Google Play</span>
                        </span>
                    </button>

                    <button class="flex justify-between items-center bg-blue-500 px-4 py-2 rounded-xl gap-2 ">
                        <svg xmlns="http://www.w3.org/2000/svg" viewBox="0 0 24 24" class="w-10 fill-current">
                            <path
                                d="M18.71,19.5C17.88,20.74 17,21.95 15.66,21.97C14.32,22 13.89,21.18 12.37,21.18C10.84,21.18 10.37,21.95 9.1,22C7.79,22.05 6.8,20.68 5.96,19.47C4.25,17 2.94,12.45 4.7,9.39C5.57,7.87 7.13,6.91 8.82,6.88C10.1,6.86 11.32,7.75 12.11,7.75C12.89,7.75 14.37,6.68 15.92,6.84C16.57,6.87 18.39,7.1 19.56,8.82C19.47,8.88 17.39,10.1 17.41,12.63C17.44,15.65 20.06,16.66 20.09,16.67C20.06,16.74 19.67,18.11 18.71,19.5M13,3.5C13.73,2.67 14.94,2.04 15.94,2C16.07,3.17 15.6,4.35 14.9,5.19C14.21,6.04 13.07,6.7 11.95,6.61C11.8,5.46 12.36,4.26 13,3.5Z" />
                        </svg>
                        <span class="flex flex-col justify-start text-left">
                            <span class=" uppercase text-xs">Get in on </span>
                            <span class=" text-2xl">Apple Store</span>
                        </span>
                    </button>

                </div>
            </div>
        </div>


        <div class="absolute w-1/2 h-full right-0 top-10 grid grid-cols-12 gap-2">

            <div class="h-40 bg-gray-400/20 col-start-1 col-end-3 "></div>
            <div class="h-40 bg-gray-400/20 col-start-3 col-end-8 "></div>
            <div class="h-40 bg-gray-400/20 col-start-8 col-end-12 "></div>

            <div class="h-56 bg-gray-400/20 row-start-2  col-start-1 col-end-7 "></div>
            <div class="h-56 bg-gray-400/20 col-start-7 col-end-12 "></div>

            <div class="h-56 bg-gray-400/20 row-start-3 col-start-1 col-end-3 "></div>
            <div class="h-56 bg-gray-400/20 col-start-3 col-end-8 "></div>
            <div class="h-56 bg-gray-400/20 col-start-8 col-end-12 "></div>

        </div>

        <div class="absolute bottom-0 left-72 flex items-center gap-4">
            <svg xmlns="http://www.w3.org/2000/svg" width="32" height="32" viewBox="0 0 24 24" class="w-8 animate-bounce">
                <path fill="currentColor" fill-rule="evenodd"
                    d="M4.25 9a7.75 7.75 0 1 1 15.5 0v6a7.75 7.75 0 0 1-15.5 0zM12 2.75A6.25 6.25 0 0 0 5.75 9v6a6.25 6.25 0 1 0 12.5 0V9A6.25 6.25 0 0 0 12 2.75m0 1.5a.75.75 0 0 1 .75.75v3a.75.75 0 0 1-1.5 0V5a.75.75 0 0 1 .75-.75"
                    clip-rule="evenodd" />
            </svg>
            <span>
                Scroll Down
            </span>


        </div>



    </section>

</template>

