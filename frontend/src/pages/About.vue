<!-- <template>
    <Navbar />
    <div class="min-h-auto bg-[#090c14] flex items-center justify-center p-4">
        <div class="w-full  bg-[#121826] rounded-2xl shadow-lg flex flex-col md:flex-row">
            <div class="w-full md:w-2/3 p-6 md:p-10 text-white">
                <h1 class="text-3xl font-bold mb-4">About Me</h1>
                <p class="text-gray-300 leading-relaxed">
                    My name is Prabhakar Kumar. I am a Frontend Developer. When I
                    passed 10th, I became interested in App Development due to which I
                    started learning Programming Languages. First of all I started learning
                    Java language. After learning it till intermediate I came to know that
                    Google has created a language called Kotlin for App Development
                    and then I started learning Kotlin. I learned about the basics needed
                    to develop an App and then created one or two smaller Apps. Later I
                    chose web development for a few reasons. After learning HTML, CSS
                    and JavaScript, I also created 5-6 projects. After that came my 12th
                    final exams due to which I stayed away from Web Development for a
                    few months. After the exams were over, I moved ahead with my Web
                    Development journey.
                </p>

                <div class="mt-6 flex space-x-4">
                    <button class="bg-[#1e293b] text-white px-4 py-2 rounded-lg flex items-center space-x-2">
                        <svg xmlns="http://www.w3.org/2000/svg" class="h-5 w-5" viewBox="0 0 20 20" fill="currentColor">
                            <path fill-rule="evenodd"
                                d="M6 6V5a3 3 0 013-3h2a3 3 0 013 3v1h2a2 2 0 012 2v3.57A22.952 22.952 0 0110 13a22.95 22.95 0 01-8-1.43V8a2 2 0 012-2h2zm2-1a1 1 0 011-1h2a1 1 0 011 1v1H8V5zm1 5a1 1 0 011-1h.01a1 1 0 110 2H10a1 1 0 01-1-1z"
                                clip-rule="evenodd" />
                            <path
                                d="M2 13.692V16a2 2 0 002 2h12a2 2 0 002-2v-2.308A24.254 24.254 0 0110 15c-2.75 0-5.455-.477-8-1.308z" />
                        </svg>
                        <span>02+ Years Experience</span>
                    </button>
                    <button class="bg-[#1e293b] text-white px-4 py-2 rounded-lg flex items-center space-x-2">
                        <svg xmlns="http://www.w3.org/2000/svg" class="h-5 w-5" viewBox="0 0 20 20" fill="currentColor">
                            <path
                                d="M10.394 2.08a1 1 0 00-.788 0l-7 3a1 1 0 000 1.84L5.25 8.051a.999.999 0 01.356-.257l4-1.714a1 1 0 11.788 1.838L7.667 9.088l1.94.831a1 1 0 00.787 0l7-3a1 1 0 000-1.838l-7-3z" />
                            <path
                                d="M3.223 10.481a1 1 0 01.515.927v4.132l3.2 1.36a1 1 0 00.787 0l4-1.714a1 1 0 00.6-.925V8.432l-4 1.715a1 1 0 01-.787 0L3.223 8.57V10.48zM12.54 16.114l4-1.714a1 1 0 00.6-.925V6.294a1 1 0 00-1.302-.976l-4 1.405v5.139a1 1 0 01-.6.925z" />
                        </svg>
                        <span>BCA Bachelors Degree</span>
                    </button>
                </div>
            </div>

            <div class="w-full md:w-1/3 flex items-center justify-center p-6">
                <div class="relative">
                    <div
                        class="absolute inset-0 bg-gradient-to-br from-cyan-400 to-blue-500 rounded-2xl transform rotate-3 scale-105">
                    </div>
                    <img :src="profileImage" alt="Profile"
                        class="relative z-10 w-64 h-64 object-cover rounded-2xl transform -rotate-3" />
                </div>
            </div>
        </div>
    </div>
</template>

<script setup>
import Navbar from '../components/Navbar.vue';

import { ref } from 'vue'

const profileImage = ref('/path-to-your-image.jpg')
</script> -->


<template>
    <Navbar />
    <div class="min-h-screen bg-[#04152D] text-white flex items-center justify-center p-4">
        <div class="max-w-6xl w-full flex flex-col md:flex-row items-center gap-8">

            <div class="w-full md:w-1/2  bg-orange-600">
                <div>
                    <img src="" alt="" class="mx-auto rounded shadow-lg object-cover h-[500px] w-full" />
                    <!-- <img src="https://res.cloudinary.com/deuh2cmub/image/upload/v1745842835/Vivek_a4cbqt.jpg" alt=""
                        class="mx-auto rounded shadow-lg object-cover h-[500px] w-full" /> -->
                </div>
                <div class="absolute inset-0 bg-gradient-to-r from-transparent to-[#04152D] opacity-50 z-0"></div>
            </div>

            <div class="w-full md:w-2/3">

                <div class="mb-10 ">
                    <span class="text-[36px] font-bold">About </span>
                    <span class="text-orange-500 text-[36px] font-bold">Me</span>
                    <p class="text-gray-300 text-lg mb-4 font-semibold pl-6">
                        My Introduction
                    </p>
                </div>
                <p class="text-gray-300 leading-relaxed mb-20">
                    My name is Vivek Kumar. I am a Frontend Developer & UX / UI Designer. When I
                    passed 10th, I became interested in App Development due to which I
                    started learning Programming Languages. First of all I started learning
                    Java language. After learning it till intermediate I came to know that
                    Google has created a language called Kotlin for App Development
                    and then I started learning Kotlin. I learned about the basics needed
                    to develop an App and then created one or two smaller Apps. Later I
                    chose web development for a few reasons. After learning HTML, CSS
                    and JavaScript, I also created 5-6 projects. After that came my 12th
                    final exams due to which I stayed away from Web Development for a
                    few months. After the exams were over, I moved ahead with my Web
                    Development journey
                </p>

                <div class="flex flex-col md:flex-row gap-4 justify-center items-center p-4 mb-40">
                    <div class="w-full max-w-xs ">
                        <div class="rounded-2xl p-4 flex items-center space-x-4 shadow-lg border ">
                            <div class="bg-[#2563EB] rounded-full p-2 inline-flex items-center justify-center">
                                <svg xmlns="http://www.w3.org/2000/svg" class="h-6 w-6" viewBox="0 0 20 20"
                                    fill="currentColor">
                                    <path fill-rule="evenodd"
                                        d="M6 6V5a3 3 0 013-3h2a3 3 0 013 3v1h2a2 2 0 012 2v3.57A22.952 22.952 0 0110 13a22.95 22.95 0 01-8-1.43V8a2 2 0 012-2h2zm2-1a1 1 0 011-1h2a1 1 0 011 1v1H8V5zm1 5a1 1 0 011-1h.01a1 1 0 110 2H10a1 1 0 01-1-1z"
                                        clip-rule="evenodd" />
                                    <path
                                        d="M2 13.692V16a2 2 0 002 2h12a2 2 0 002-2v-2.308A24.254 24.254 0 0110 15c-2.75 0-5.455-.477-8-1.308z" />
                                </svg>
                            </div>
                            <div>
                                <h3 class="text-white text-lg font-semibold">Experience</h3>
                                <p class="text-gray-400 text-md">02+ Years</p>
                            </div>
                        </div>
                    </div>

                    <div class="w-full max-w-xs">
                        <div class="rounded-2xl p-4 flex items-center space-x-4 shadow-lg border h-[200]">
                            <div class="bg-[#10B981] rounded-full p-2 inline-flex items-center justify-center">
                                <svg xmlns="http://www.w3.org/2000/svg" class="h-6 w-6 text-white" fill="none"
                                    viewBox="0 0 24 24" stroke="currentColor">
                                    <path stroke-linecap="round" stroke-linejoin="round" stroke-width="2"
                                        d="M12 6.253v13m0-13C10.832 5.477 9.246 5 7.5 5S4.168 5.477 3 6.253v13C4.168 18.477 5.754 18 7.5 18s3.332.477 4.5 1.253m0-13C13.168 5.477 14.754 5 16.5 5c1.747 0 3.332.477 4.5 1.253v13C19.832 18.477 18.246 18 16.5 18c-1.746 0-3.332.477-4.5 1.253" />
                                </svg>
                            </div>
                            <div>
                                <h3 class="text-white text-lg font-semibold">Education</h3>
                                <p class="text-gray-400 text-md">BCA Bachelors Degree</p>
                            </div>
                        </div>
                    </div>
                </div>
            </div>
        </div>
    </div>
</template>

<script setup>
import Navbar from '../components/Navbar.vue';
</script>
