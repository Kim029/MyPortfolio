<script setup>
// Social Links - Update this links to your link
const FacebookLink = 'https://www.facebook.com/idgaf9111';
const LinkedinLink = 'https://www.linkedin.com/in/ravina-rachiel-j-7a317a2b5/';



</script>

<template>
    <section class="flex flex-col justify-between gap-6 sm:gap-10 md:gap-16 lg:flex-row py-2">
        <!-- content - start -->
        <div class="flex flex-col justify-between xl:w-5/12">
            <div></div>

            <div class="sm:text-center lg:py-12 lg:text-left xl:py-24">
                <p class="mb-4 font-semibold text-gray-100 md:mb-6 md:text-lg xl:text-xl">Getting to know</p>

                <h1 class="mb-8 text-4xl font-bold text-gray-200 sm:text-5xl md:mb-12">Hi, I'm <br> Rachiel Ravina, <br> a BSIT student.</h1>

                <div class="flex flex-col gap-2.5 sm:flex-row sm:justify-center lg:justify-start">
                    <router-link to="/about" href="#"
                        class="inline-block rounded-lg bg-violet-700 px-8 py-3 text-center text-sm font-semibold text-white outline-none 
                        ring-indigo-300 transition duration-100 hover:bg-cyan-600 focus-visible:ring active:bg-cyan-700 md:text-base">
                        About Me
                    </router-link>

                    <router-link to="/contact"
                        class="inline-block rounded-lg bg-gray-200 px-8 py-3 text-center text-sm font-semibold text-gray-500 outline-none 
                        ring-indigo-300 transition duration-100 hover:bg-gray-300 focus-visible:ring active:text-gray-700 md:text-base">
                        Contact Me
                    </router-link>
                </div>
            </div>

            <!-- Social Media -->
            <div class="text-gray-200 mt-8 flex items-center justify-center gap-4 sm:mt-16 lg:justify-start">
                <span class="text-sm font-semibold uppercase tracking-widest text-gray-100 sm:text-base">Social</span>
                <span class="h-px w-12 bg-gray-200"></span>

                <div class="flex gap-4">
                    <a :href="FacebookLink" target="_blank" 
                        class="text-gray-200 transition duration-100 hover:text-gray-500 active:text-gray-600">
                        <svg class="h-5 w-5" aria-hidden="true" xmlns="http://www.w3.org/2000/svg"
                            fill="currentColor" viewBox="0 0 8 19">
                            <path fill-rule="evenodd"
                                d="M6.135 3H8V0H6.135a4.147 4.147 0 0 0-4.142 4.142V6H0v3h2v9.938h3V9h2.021l.592-3H5V3.591A.6.6 0 0 1 5.592 3h.543Z"
                                clip-rule="evenodd" />
                        </svg>
                    </a>

                    <a :href="LinkedinLink" target="_blank"
                        class="text-gray-200 transition duration-100 hover:text-gray-500 active:text-gray-600">
                        <svg class="h-5 w-5" width="24" height="24" viewBox="0 0 24 24" fill="currentColor"
                            xmlns="http://www.w3.org/2000/svg">
                            <path
                                d="M19 0h-14c-2.761 0-5 2.239-5 5v14c0 2.761 2.239 5 5 5h14c2.762 0 5-2.239 5-5v-14c0-2.761-2.238-5-5-5zm-11 19h-3v-11h3v11zm-1.5-12.268c-.966 0-1.75-.79-1.75-1.764s.784-1.764 1.75-1.764 1.75.79 1.75 1.764-.783 1.764-1.75 1.764zm13.5 12.268h-3v-5.604c0-3.368-4-3.113-4 0v5.604h-3v-11h3v1.765c1.396-2.586 7-2.777 7 2.476v6.759z" />
                        </svg>
                    </a>
                </div>
            </div>
        </div>
        <div class="background-image-container">
            <img src="https://scontent.fceb3-1.fna.fbcdn.net/v/t1.15752-9/423454983_1105417480495767_8919237847726397319_n.png?_nc_cat=103&ccb=1-7&_nc_sid=5f2048&_nc_eui2=AeFGQGlkSkWgPzk_MzsCpkj9e4g1YdaXuQ97iDVh1pe5DxIumulgHb-LpSLlxOqIfvDYfkDqSc-gIPvfoWaZNBYJ&_nc_ohc=Dzgd30d1UswQ7kNvgF69CPL&_nc_oc=Adh_rr4dtUIgFoiQV1T4yiaWAl-lX8VRbzzDl1vYxAidPfAjSw4dUo3AkCceaMDEeYg&_nc_ht=scontent.fceb3-1.fna&oh=03_Q7cD1QE65lN_pC0vmgS1CZs2ZvYONu6ZR6qjKkRoBwYpGxb5ZQ&oe=66556A8A"
                loading="" alt="" class="h-full w-full object-cover object-center" />
        </div>

    </section>
</template>
