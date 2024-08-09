<script setup>
import { ref } from 'vue'
const content = ref([
    {
        title: 'More than just a music player',
        description: 'Lorem ipsum dolor sit amet, consectetur adipiscing elit. Nullam auctor, nunc nec'
    },
    {
        title: 'More than just a music player',
        description: 'Lorem ipsum dolor sit amet, consectetur adipiscing elit. Nullam auctor, nunc nec'
    },
    {
        title: 'More than just a music player',
        description: 'Lorem ipsum dolor sit amet, consectetur adipiscing elit. Nullam auctor, nunc nec'
    },
])

</script>

<template>
    <section class="py-20">
        <div class="container rounded-2xl bg-slate-50 dark:bg-indigo-800/20 py-10 space-y-7 px-20 ">
            <h2 class=" text-5xl text-center">
                More than just a music player
            </h2>

            <div class="flex justify-between items-start gap-10">
                <div class="flex-1 gap-y-32 flex flex-col py-36">
                    <div v-for="({ title, description }, index) in content" :key="index" class="space-y-7 max-w-sm">
                        <p class="w-10 h-10  flex justify-center items-center rounded-full"
                            :class="index === 0 ? 'bg-blue-500 text-white' : 'bg-indigo-50 text-indigo-900'">
                            {{ index + 1 }}
                        </p>
                        <h3 class="text-xl font-bold">
                            {{ title }}
                        </h3>
                        <p>
                            {{ description }}
                        </p>
                    </div>

                </div>

                <div class="flex-1 flex flex-col py-10">
                    <div class="h-96 max-w-sm bg-indigo-200 relative">
                        <div
                            class="absolute top-10 -right-10 bg-white dark:bg-indigo-950 flex justify-between items-center rounded-xl overflow-hidden">
                            <div class="px-7">
                                <p class="font-bold ">
                                    Morning Playlist
                                </p>
                                <p class="font-thin">
                                    The best songs ever.
                                </p>
                            </div>
                            <img src="https://img.freepik.com/free-photo/still-life-wireless-cyberpunk-headphones_23-2151072204.jpg?t=st=1723202677~exp=1723206277~hmac=6d5558f2df6ca40c8275b9bfba3381966dcb2d92014816b841d00a9fed4878f6&w=800"
                                alt="" class="w-20 h-20 bg-pink-50">
                        </div>
                    </div>
                </div>
            </div>
        </div>
    </section>


</template>
