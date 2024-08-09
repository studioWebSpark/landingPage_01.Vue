<template>
    <section class="py-20 bg-slate-200/20 dark:bg-indigo-800/10">
        <div class="container space-y-20">
            <div class="text-center space-y-3">
                <p>
                    Join tens of thousands of creators, artists, and listeners who are using Tonality to share their
                </p>
                <h2 class="text-5xl">
                    What our users are saying
                </h2>
            </div>

            <div class="mx-auto container flex items-center  gap-7">
                <div class="flex flex-col items-center space-y-4 w-96 bg-white dark:bg-indigo-950 rounded-xl shadow dark:shadow-indigo-800 p-8"
                    v-for="i in 4" :key="i">
                    <img src="https://img.freepik.com/free-photo/overjoyed-teenage-girl-with-curly-combed-hair-makes-yes-gesture-keeps-fists-raised-up-celebrates-successfully_273609-52682.jpg?t=st=1723214367~exp=1723217967~hmac=4ed23b14c30b14939769e0ea3ab1423a966ac9be4ec7375e8680f95c29f30e5f&w=1000"
                        alt="John Doe" class="w-24 h-24 rounded-full">
                    <p class="text-xl font-semibold">
                        Marge Doe
                    </p>
                    <p class="text-sm text-gray-500"> CEO at Company</p>
                    <p class="font-bold">Amazing sound!</p>
                    <p class="text-sm text-gray-600 dark:text-indigo-200 text-center">
                        "Lorem ipsum dolor sit amet, consectetur adipiscing elit. Nullam auctor, nunc nec"
                    </p>
                    <div class="flex justify-center items-center">
                        <svg v-for="i in 5" :key="i" xmlns="http://www.w3.org/2000/svg" viewBox="0 0 24 24"
                            class="w-6 fill-current text-yellow-500">
                            <path
                                d="M12,2L15.09,8.26L22,9.24L17,14.14L18.18,21L12,17.27L5.82,21L7,14.14L2,9.24L8.91,8.26L12,2Z" />

                            >

                            <path
                                d="M12,17.27L18.18,21L16.54,13.97L22,9.24L14.81,8.62L12,2L9.19,8.62L2,9.24L7.45,13.97L5.82,21L12,17.27Z" />
                        </svg>

                    </div>
                </div>

            </div>
        </div>

    </section>
</template>