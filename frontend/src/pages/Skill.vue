<!-- <template>
    <div class="min-h-screen bg-blue-900 text-white flex flex-col justify-center items-center px-4">
        <h1 class="text-[36px] font-bold mb-2">
            My <span class="text-cyan-400 text-[36px] font-bold">Skills</span>
        </h1>
        <p class="text-lg mb-6">My Expertise</p>
        <div class="grid grid-cols-1 sm:grid-cols-2 lg:grid-cols-3 gap-6">
            <div class="flex flex-col items-center bg-blue-800 p-4 rounded-2xl shadow-lg">
                <img src="..//assets/Inter/Figma.png" alt="" class="w-12 h-12 mb-2" />
                <h2 class="text-xl font-semibold">Figma</h2>
                <p class="text-sm text-gray-300">Intermediate</p>
            </div>
            <div class="flex flex-col items-center bg-blue-800 p-4 rounded-2xl shadow-lg">
                <img src="..//assets/Inter/Html.png" alt="" class="w-12 h-12 mb-2" />
                <h2 class="text-xl font-semibold">HTML</h2>
                <p class="text-sm text-gray-300">Experienced</p>
            </div>
            <div class="flex flex-col items-center bg-blue-800 p-4 rounded-2xl shadow-lg">
                <img src="..//assets/Inter/Css.png" alt="" class="w-12 h-12 mb-2" />
                <h2 class="text-xl font-semibold">CSS</h2>
                <p class="text-sm text-gray-300">Experienced</p>
            </div>
            <div class="flex flex-col items-center bg-blue-800 p-4 rounded-2xl shadow-lg">
                <img src="..//assets/Inter/Javascript.png" alt="" class="w-12 h-12 mb-2" />
                <h2 class="text-xl font-semibold">JavaScript</h2>
                <p class="text-sm text-gray-300">Intermediate</p>
            </div>
            <div class="flex flex-col items-center bg-blue-800 p-4 rounded-2xl shadow-lg">
                <img src="..//assets/Inter/React.png" alt="" class="w-12 h-12 mb-2" />
                <h2 class="text-xl font-semibold">React js</h2>
                <p class="text-sm text-gray-300">Intermediate</p>
            </div>
            <div class="flex flex-col items-center bg-blue-800 p-4 rounded-2xl shadow-lg">
                <img src="..//assets/Inter/Git.png" alt="" class="w-12 h-12 mb-2" />
                <h2 class="text-xl font-semibold">Git</h2>
                <p class="text-sm text-gray-300">Basic</p>
            </div>
            <div class="flex flex-col items-center bg-blue-800 p-4 rounded-2xl shadow-lg">
                <img src="..//assets/Inter/Github.png" alt="" class="w-12 h-12 mb-2" />
                <h2 class="text-xl font-semibold">GitHub</h2>
                <p class="text-sm text-gray-300">Basic</p>
            </div>

        </div>
    </div>
</template>

<script setup>

</script>

<style scoped></style> -->

<!-- 
<template>
    <Navbar />

    <div class="min-h-screen bg-blue-900 text-white flex flex-col justify-center items-center px-4">
        <h1 class="text-[36px] font-bold mb-2">
            My <span class="text-[36px] font-bold text-cyan-400">Skills</span>
        </h1>
        <p class="text-lg mb-6">My Expertise</p>
        <div class="grid grid-cols-1 sm:grid-cols-2 lg:grid-cols-3 gap-6 ">
            <div v-for="skill in skills" :key="skill.name"
                class="flex flex-col items-center bg-blue-800 p-4 rounded-2xl shadow-lg">
                <img :src="skill.icon" :alt="skill.name" class="w-12 h-12 mb-2" />
                <h2 class="text-xl font-semibold">{{ skill.name }}</h2>
                <p class="text-sm text-gray-300">{{ skill.level }}</p>
            </div>
        </div>
    </div>
</template>

<script setup>
import Navbar from '../components/Navbar.vue';


const skills = [
    { name: 'Figma', level: 'Intermediate', icon: 'https://cdn.iconscout.com/icon/free/png-256/free-figma-logo-icon-download-in-svg-png-gif-file-formats--technology-social-media-vol-3-pack-logos-icons-3030133.png?f=webp&w=256' },
    { name: 'HTML', level: 'Experienced', icon: 'https://cdn.iconscout.com/icon/free/png-256/free-html-5-logo-icon-download-in-svg-png-gif-file-formats--programming-langugae-language-pack-logos-icons-1175208.png?f=webp&w=256' },
    { name: 'CSS', level: 'Experienced', icon: 'https://cdn.worldvectorlogo.com/logos/css-3.svg' },
    { name: 'JavaScript', level: 'Intermediate', icon: 'https://i.pinimg.com/736x/13/40/7c/13407c12f50f08d328800c3caef43f61.jpg' },
    { name: 'React.js', level: 'Intermediate', icon: 'https://cdn4.iconfinder.com/data/icons/logos-3/600/React.js_logo-512.png' },
    { name: 'Git', level: 'Basic', icon: 'https://git-scm.com/images/logos/downloads/Git-Icon-1788C.png' },
    { name: 'GitHub', level: 'Basic', icon: 'https://cdn2.iconfinder.com/data/icons/font-awesome/1792/github-512.png' },
    { name: 'Frappe', level: 'Basic', icon: 'https://docs.frappe.io/files/framework.svg' },

];
</script>

<style scoped></style> -->


<template>
    <Navbar />
    <div class="min-h-screen max-w-4xl mx-auto px-4 py-8 pt-32">
        <h1 class="text-[28px] font-bold text-center mb-16">Skills & Technologies</h1>

        <div class="grid grid-cols-1 md:grid-cols-2 gap-x-12 gap-y-10">
            <div v-for="(skill, index) in skills" :key="index" class="skill-item">
                <div class="flex justify-between mb-2">
                    <span class="font-medium">{{ skill.name }}</span>
                    <span>{{ skill.percentage }}%</span>
                </div>
                <div class="h-2 bg-gray-200 rounded-full">
                    <div class="h-full bg-blue-600 rounded-full" :style="{ width: `${skill.percentage}%` }"></div>
                </div>
            </div>
        </div>
    </div>
</template>

<script setup>
import { ref } from 'vue';
import Navbar from '../components/Navbar.vue';


const skills = ref([
    { name: 'HTML', percentage: 90 },
    { name: 'CSS', percentage: 85 },
    { name: 'Tailwind CSS', percentage: 90 },
    { name: 'JavaScript', percentage: 85 },
    { name: 'TypeScript', percentage: 80 },
    { name: 'React', percentage: 90 },
    { name: 'Node.js', percentage: 75 },
    { name: 'Vue js', percentage: 75 },
    { name: 'Git', percentage: 80 },
    { name: 'Frappe', percentage: 80 },
    { name: 'Figma', percentage: 80 },
]);
</script>

<style scoped></style>
