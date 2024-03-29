<script setup>
import { ref } from 'vue';

const isOpenMenu = ref(false);

// Social Links - Update this links to your link
const FacebookLink = 'https://www.facebook.com/idgaf9111';
const LinkedinLink = 'https://www.linkedin.com/in/ravina-rachiel-j-7a317a2b5/';


const toggleMobileMenu = () => {
    return isOpenMenu.value = !isOpenMenu.value;
};

</script>

<template>
    <header class="bg-dark border-b border-gray-200">
        <nav class="mx-auto max-w-screen-xl px-12 py-4">
            <div class="flex flex-row items-center justify-between">
                <router-link to="/" class="flex flex-col">
                    <h1 class="text-gray-200 font-bold text-xl">Rachiel Ravina</h1>
                </router-link>

                <!-- Desktop Menu -->
                <div class="hidden lg:block">
                    <ul class="flex flex-row gap-8">
                        <li
                            :class="$route.name === 'home' ? 'text-gray-200 text-cyan-200 font-medium text-lg' : 'text-gray-200 hover:text-cyan-700 font-normal text-lg'">
                            <router-link to="/">Home</router-link>
                        </li>
                        <li
                            :class="$route.name === 'about' ? 'text-gray-200 text-cyan-200 font-medium text-lg' : 'text-gray-200 hover:text-cyan-700 font-normal text-lg'">
                            <router-link to="/about">About</router-link>
                        </li>
                        <li
                            :class="$route.name === 'projects' ? 'text-gray-200 text-cyan-200 font-medium text-lg' : 'text-gray-200 hover:text-cyan-700 font-normal text-lg'">
                            <router-link to="/projects">Skills</router-link>
                        </li>
                        <li
                            :class="$route.name === 'contact' ? 'text-gray-200 text-cyan-200 font-medium text-lg' : 'text-gray-200 hover:text-cyan-700 font-normal text-lg'">
                            <router-link to="/contact">Contact</router-link>
                        </li>
                    </ul>
                </div>

                <!-- Desktop Social Icons -->
                <div class="hidden lg:block">
                    <ul class="flex flex-row items-center gap-3">
                        <a :href="FacebookLink" target="_blank" class="bg-gray-100 hover:bg-gray-300 p-2 rounded-full">
                            <svg class="w-[20px] h-[20px] text-gray-600" aria-hidden="true"
                                xmlns="http://www.w3.org/2000/svg" fill="currentColor" viewBox="0 0 8 19">
                                <path fill-rule="evenodd"
                                    d="M6.135 3H8V0H6.135a4.147 4.147 0 0 0-4.142 4.142V6H0v3h2v9.938h3V9h2.021l.592-3H5V3.591A.6.6 0 0 1 5.592 3h.543Z"
                                    clip-rule="evenodd" />
                            </svg>
                        </a>
                        <a :href="LinkedinLink" target="_blank" class="bg-gray-100 hover:bg-gray-300 p-2 rounded-full">
                            <svg class="w-[20px] h-[20px] text-gray-600" aria-hidden="true"
                                xmlns="http://www.w3.org/2000/svg" fill="currentColor" viewBox="0 0 15 15">
                                <path fill-rule="evenodd"
                                    d="M7.979 5v1.586a3.5 3.5 0 0 1 3.082-1.574C14.3 5.012 15 7.03 15 9.655V15h-3v-4.738c0-1.13-.229-2.584-1.995-2.584-1.713 0-2.005 1.23-2.005 2.5V15H5.009V5h2.97ZM3 2.487a1.5 1.5 0 1 1-3 0 1.5 1.5 0 0 1 3 0Z"
                                    clip-rule="evenodd" />
                                <path d="M3 5.012H0V15h3V5.012Z" />
                            </svg>
                        </a>
                    </ul>
                </div>

                <!-- Burger Menu -->
                <div @click="toggleMobileMenu"
                    class="cursor-pointer block lg:hidden border border-gray-200 bg-gray-100 hover:bg-gray-200 p-2 rounded-full">
                    <svg class="w-[24px] h-[24px] text-gray-700" aria-hidden="true" xmlns="http://www.w3.org/2000/svg"
                        fill="none" viewBox="0 0 16 12">
                        <path stroke="currentColor" stroke-linecap="round" stroke-linejoin="round" stroke-width="1.5"
                            d="M1 1h14M1 6h14M1 11h7" />
                    </svg>
                </div>
            </div>

            <!-- Mobile Menu -->
            <div v-if="isOpenMenu" class="flex lg:hidden relative">

                <div class="bg-gray-200 flex flex-col absolute top-[18px] -left-[52px] w-screen gap-4 shadow-lg p-6 rounded">
                    <router-link to="/"
                        :class="$route.name === 'home' ? 'bg-gr-50 p-2 rounded text-cyan-700 font-medium text-lg' : 'hover:bg-gray-50 p-2 text-gray-700 hover:text-cyan-700 font-normal text-lg'">
                        Home
                    </router-link>
                    <router-link to="/about"
                        :class="$route.name === 'about' ? 'bg-gray-50 p-2 rounded text-cyan-700 font-medium text-lg' : 'hover:bg-gray-50 p-2 text-gray-700 hover:text-cyan-700 font-normal text-lg'">
                        About
                    </router-link>
                    <router-link to="/projects"
                        :class="$route.name === 'projects' ? 'bg-gray-50 p-2 rounded text-cyan-700 font-medium text-lg' : 'hover:bg-gray-50 p-2 text-gray-700 hover:text-cyan-700 font-normal text-lg'">
                        Skills
                    </router-link>
                    <router-link to="/contact"
                        :class="$route.name === 'contact' ? 'bg-gray-50 p-2 rounded text-cyan-700 font-medium text-lg' : 'hover:bg-gray-50 p-2 text-gray-700 hover:text-cyan-700 font-normal text-lg'">
                        Contact
                    </router-link>

                    <!-- Mobile Social Icons -->
                    <ul class="flex flex-row items-center gap-3 mt-2">
                        <a :href="FacebookLink" target="_blank" class="bg-gray-100 hover:bg-gray-300 p-2 rounded-full">
                            <svg class="w-[20px] h-[20px] text-gray-600" aria-hidden="true"
                                xmlns="http://www.w3.org/2000/svg" fill="currentColor" viewBox="0 0 8 19">
                                <path fill-rule="evenodd"
                                    d="M6.135 3H8V0H6.135a4.147 4.147 0 0 0-4.142 4.142V6H0v3h2v9.938h3V9h2.021l.592-3H5V3.591A.6.6 0 0 1 5.592 3h.543Z"
                                    clip-rule="evenodd" />
                            </svg>
                        </a>
                        <a :href="LinkedinLink" target="_blank" class="bg-gray-100 hover:bg-gray-300 p-2 rounded-full">
                            <svg class="w-[20px] h-[20px] text-gray-600" aria-hidden="true"
                                xmlns="http://www.w3.org/2000/svg" fill="currentColor" viewBox="0 0 15 15">
                                <path fill-rule="evenodd"
                                    d="M7.979 5v1.586a3.5 3.5 0 0 1 3.082-1.574C14.3 5.012 15 7.03 15 9.655V15h-3v-4.738c0-1.13-.229-2.584-1.995-2.584-1.713 0-2.005 1.23-2.005 2.5V15H5.009V5h2.97ZM3 2.487a1.5 1.5 0 1 1-3 0 1.5 1.5 0 0 1 3 0Z"
                                    clip-rule="evenodd" />
                                <path d="M3 5.012H0V15h3V5.012Z" />
                            </svg>
                        </a>
                    </ul>
                </div>
            </div>
        </nav>
    </header>
</template>