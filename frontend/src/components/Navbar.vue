<!-- <template>
    <nav class="bg-blue-900 text-white">
        <div class="max-w-7xl mx-auto px-4 sm:px-6 lg:px-8">
            <div class="flex justify-between items-center h-16">
                <div class="flex items-center">
                    <span class="text-xl font-bold tracking-wide">
                        <span class="text-white">VIVEK</span><span class="text-teal-500"> KUMAR</span>
                    </span>
                </div>
                <div class="hidden md:flex space-x-8">
                    <a href="#" class="text-white hover:text-teal-400 transition">HOME</a>
                    <a href="#" class="text-white hover:text-teal-400 transition">ABOUT</a>
                    <a href="#" class="text-white hover:text-teal-400 transition">SKILLS</a>
                    <a href="#" class="text-white hover:text-teal-400 transition">PROJECTS</a>
                    <a href="#" class="text-white hover:text-teal-400 transition">CONTACT</a>
                </div>
               
                <div class="flex md:hidden">
                    <button @click="isMenuOpen = !isMenuOpen" class="text-white focus:outline-none">
                        <svg class="h-6 w-6" fill="none" stroke="currentColor" viewBox="0 0 24 24"
                            xmlns="http://www.w3.org/2000/svg">
                            <path stroke-linecap="round" stroke-linejoin="round" stroke-width="2"
                                d="M4 6h16M4 12h16m-7 6h7"></path>
                        </svg>
                    </button>
                </div>
            </div>
        </div>
        
        <div v-if="isMenuOpen" class="md:hidden bg-blue-800">
            <a href="#" class="block px-4 py-2 text-white hover:bg-teal-600">HOME</a>
            <a href="/about" class="block px-4 py-2 text-white hover:bg-teal-600">ABOUT</a>
            <a href="/skill" class="block px-4 py-2 text-white hover:bg-teal-600">SKILLS</a>
            <a href="/projects" class="block px-4 py-2 text-white hover:bg-teal-600">PROJECTS</a>
            <a href="/contact" class="block px-4 py-2 text-white hover:bg-teal-600">CONTACT</a>
        </div>
    </nav>
</template>

<script setup>
import { ref } from 'vue';

const isMenuOpen = ref(false);
</script>

<style>
</style> -->



<template>
    <nav class="fixed top-0 left-0 w-full bg-[#04152D] flex items-center justify-between px-4 py-3 z-50">
        <!-- Logo -->
        <div class="text-orange-500 font-bold text-xl">LOGO</div>

        <!-- Desktop Navigation -->
        <div class="hidden md:flex items-center space-x-6">
            <a href="/" class="text-white hover:text-orange-500 transition-colors">HOME</a>
            <!-- <a href="/about" class="text-white hover:text-orange-500 transition-colors">ABOUT ME</a> -->
            <nav class="text-white hover:text-orange-500 transition-colors">
                <a @click.prevent="scrollTo('about')">ABOUT ME</a>
            </nav>
            <!-- <a href="/skill" class="text-white hover:text-orange-500 transition-colors">SKILLS</a> -->
            <nav class="text-white hover:text-orange-500 transition-colors">
                <a @click.prevent="scrollTo('skill')">SKILLS</a>
            </nav>
            <!-- <a href="/project" class="text-white hover:text-orange-500 transition-colors">PROJECTS</a> -->
            <nav class="text-white hover:text-orange-500 transition-colors">
                <a @click.prevent="scrollTo('project')">PROJECTS</a>
            </nav>
            <!-- <a href="/contact" class="text-white hover:text-orange-500 transition-colors">CONTACT ME</a> -->
            <nav class="text-white hover:text-orange-500 transition-colors">
                <a @click.prevent="scrollTo('contact')">CONTACT</a>
            </nav>
        </div>

        <!-- Mobile Menu Toggle -->
        <div class="md:hidden">
            <button @click="toggleMobileMenu" class="text-white focus:outline-none">
                <svg v-if="!mobileMenuOpen" xmlns="http://www.w3.org/2000/svg" class="h-6 w-6" fill="none"
                    viewBox="0 0 24 24" stroke="currentColor">
                    <path stroke-linecap="round" stroke-linejoin="round" stroke-width="2" d="M4 6h16M4 12h16M4 18h16" />
                </svg>
                <svg v-else xmlns="http://www.w3.org/2000/svg" class="h-6 w-6" fill="none" viewBox="0 0 24 24"
                    stroke="currentColor">
                    <path stroke-linecap="round" stroke-linejoin="round" stroke-width="2" d="M6 18L18 6M6 6l12 12" />
                </svg>
            </button>
        </div>

        <!-- Mobile Menu -->
        <div :class="[
            'fixed top-16 left-0 w-full bg-black flex-col items-center space-y-4 py-6 transition-all duration-300 ease-in-out',
            mobileMenuOpen ? 'flex' : 'hidden'
        ]">
            <a href="/" class="text-white hover:text-orange-500 transition-colors">Home</a>
            <!-- <a href="/about" class="text-white hover:text-orange-500 transition-colors">ABOUT ME</a> -->
            <nav class="text-white hover:text-orange-500 transition-colors">
                <a @click.prevent="scrollTo('about')">ABOUT ME</a>
            </nav>
            <a href="/skill" class="text-white hover:text-orange-500 transition-colors">SKILLS</a>
            <a href="/" class="text-white hover:text-orange-500 transition-colors">PROJECTS</a>
            <a href="contact" class="text-white hover:text-orange-500 transition-colors">CONTACT ME</a>
        </div>
    </nav>
</template>

<script setup>
import { ref } from 'vue'

const mobileMenuOpen = ref(false)

const scrollTo = (id) => {
    const element = document.getElementById(id)
    if (element) {
        element.scrollIntoView({ behavior: 'smooth' })
    }
}

const toggleMobileMenu = () => {
    mobileMenuOpen.value = !mobileMenuOpen.value
}
</script>

<style scoped>
html {
    scroll-behavior: smooth;
}
</style>