<script setup>
import MainLayout from '../components/MainLayout.vue';

// Page Title of Views
const pageTitle = 'Projects'
</script>

<template>
  <MainLayout :pageTitle="pageTitle">
    <section>
      <div class="bg-dark py-6 sm:py-8 lg:py-0">
        <div class="flex flex-wrap lg:flex-nowrap items-center justify-between gap-4 lg:gap-8 mb-8 md:mb-12">
            <div class="flex flex-col gap-2">
             <h2 class="text-2xl font-bold text-gray-200 lg:text-3xl">Skills</h2>
            </div>

        </div>
        
        <!-- Project Image Gallery -->
        <div class="grid grid-cols-1 gap-4 md:grid-cols-3 md:gap-6 xl:gap-8">
            <!-- image - start -->
            <router-link to="/projects" href="#" class="group relative flex h-48 items-end overflow-hidden rounded-lg bg-gray-100 shadow-lg md:h-80">
                <img src="https://b.kisscc0.com/20180815/zlq/kisscc0-computer-icons-logo-brand-javascript-angle-js-5b741783856f77.0690615715343348515466.png"
                    loading="lazy" alt="Photo by Minh Pham"
                    class="absolute inset-0 h-full w-full object-cover object-center transition duration-200 group-hover:scale-110" />

                <div
                    class="pointer-events-none absolute inset-0 bg-gradient-to-t from-gray-800 via-transparent to-transparent opacity-50">
                </div>

                <span class="relative ml-4 mb-3 inline-block text-sm text-white md:ml-5 md:text-lg">JS</span>
            </router-link>
            <!-- image - end -->

            <!-- image - start -->
            <router-link to="/projects"
                class="group relative flex h-48 items-end overflow-hidden rounded-lg bg-gray-100 shadow-lg md:col-span-2 md:h-80">
                <img src="https://www.vectorlogo.zone/logos/w3_css/w3_css-ar21.png"
                    loading="lazy" alt="Photo by Magicle"
                    class="absolute inset-0 h-full w-full object-cover object-center transition duration-200 group-hover:scale-110" />

                <div
                    class="pointer-events-none absolute inset-0 bg-gradient-to-t from-gray-800 via-transparent to-transparent opacity-50">
                </div>

                <span class="relative ml-4 mb-3 inline-block text-sm text-white md:ml-5 md:text-lg">CSS</span>
            </router-link>
            <!-- image - end -->

            <!-- image - start -->
            <router-link to="/projects"
                class="group relative flex h-48 items-end overflow-hidden rounded-lg bg-gray-100 shadow-lg md:col-span-2 md:h-80">
                <img src="https://cdn.pixabay.com/photo/2017/08/05/11/16/logo-2582748_960_720.png"
                    loading="lazy" alt="Photo by Martin Sanchez"
                    class="relative inset-0 h-full w-full object-cover object-center transition duration-200 group-hover:scale-110" />

                <div
                    class="pointer-events-none absolute inset-0 bg-gradient-to-t from-gray-800 via-transparent to-transparent opacity-50">
                </div>

                <span class="relative ml-4 mb-3 inline-block text-sm text-white md:ml-5 md:text-lg">HTML</span>
            </router-link>
            <!-- image - end -->

            <!-- image - start -->
            <router-link to="/projects" class="group relative flex h-48 items-end overflow-hidden rounded-lg bg-gray-100 shadow-lg md:h-80">
                <img src="https://miro.medium.com/v2/resize:fit:900/1*OrjCKmou1jT4It5so5gvOA.jpeg"
                    loading="lazy" alt="Photo by Lorenzo Herrera"
                    class="absolute inset-0 h-full w-full object-cover object-center transition duration-200 group-hover:scale-110" />

                <div
                    class="pointer-events-none absolute inset-0 bg-gradient-to-t from-gray-800 via-transparent to-transparent opacity-50">
                </div>
                <span class="relative ml-4 mb-3 inline-block text-sm text-white md:ml-5 md:text-lg">Vue.js</span>
            </router-link>
            <!-- image - end -->
        </div>
    </div>
    </section>
  </MainLayout>
</template>