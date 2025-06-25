<script setup>
import { ref } from 'vue';

// Props for customizing the certificate
const props = defineProps({
    recipientName: {
        type: String,
        default: 'Name Surname'
    },
    role: {
        type: String,
        default: 'A MyKartavya Volunteer'
    },
    projectName: {
        type: String,
        default: 'Project Name'
    },
    signatoryName: {
        type: String,
        default: 'Jyoti Sharma'
    },
    signatoryTitle: {
        type: String,
        default: 'CEO, NASSCOM Foundation'
    }
});
</script>
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

<style scoped></style>
<template>
    <div class="max-w-5xl mx-auto p-20"> { name: 'Frappe', level: 'Basic', icon:
        'https://docs.frappe.io/files/framework.svg' },

        <!-- Certificate with red background and circuit patterns -->
        <div class="relative bg-red-700 p-8 rounded-lg shadow-xl">
            <!-- Circuit patterns - Top right -->
            <div class="absolute top-0 right-0 w-1/3 h-20">
                <div class="border-t border-r border-white opacity-70 h-full w-full"></div>
                <div v-for="i in 6" :key="`tr-${i}`" class="absolute top-0 h-4 w-px bg-white"
                    :style="`right: ${i * 20}px; height: ${(i % 2 === 0) ? '16px' : '10px'}`">
                    <div class="absolute top-0 -right-1 h-2 w-2 rounded-full bg-white"></div>
                </div>
            </div>

            <!-- Circuit patterns - Bottom left -->
            <div class="absolute bottom-0 left-0 w-40 h-40">
                <div v-for="i in 8" :key="`bl-${i}`" class="absolute w-16 h-px bg-white"
                    :style="`bottom: ${i * 12}px; left: 0`">
                    <div class="absolute -left-1 -top-1 h-2 w-2 rounded-full bg-white"></div>
                </div>
            </div>

            <!-- Circuit patterns - Bottom right -->
            <div class="absolute bottom-0 right-0 w-40 h-48">
                <div v-for="i in 10" :key="`br-${i}`" class="absolute w-20 h-px bg-white"
                    :style="`bottom: ${i * 12}px; right: 0`">
                    <div class="absolute -right-1 -top-1 h-2 w-2 rounded-full bg-white"></div>
                </div>
            </div>

            <!-- White certificate background -->
            <div class="bg-white rounded-md p-6 sm:p-12 relative z-10">
                <!-- Top logos -->
                <div class="flex justify-end mb-8 sm:mb-12">
                    <div class="flex items-center gap-4">
                        <!-- MyKartavya logo placeholder -->
                        <div class="h-8 sm:h-10">
                            <svg width="120" height="40" viewBox="0 0 120 40" class="h-full w-auto">
                                <text x="5" y="25" fill="#e53e3e" font-size="14" font-weight="bold">MyKartavya</text>
                            </svg>
                        </div>
                        <!-- Vertical divider -->
                        <div class="h-8 border-l border-gray-300"></div>
                        <!-- NASSCOM foundation logo placeholder -->
                        <div class="h-8 sm:h-10">
                            <svg width="140" height="40" viewBox="0 0 140 40" class="h-full w-auto">
                                <text x="5" y="20" fill="#e53e3e" font-size="14" font-weight="bold">nasscom</text>
                                <text x="5" y="35" fill="#e53e3e" font-size="12">foundation</text>
                            </svg>
                        </div>
                    </div>
                </div>

                <!-- Certificate title -->
                <div class="text-center mb-8 sm:mb-12">
                    <h1 class="text-5xl sm:text-6xl font-serif text-red-700 mb-2">CERTIFICATE</h1>
                    <p class="text-xl sm:text-2xl uppercase tracking-widest">OF APPRECIATION</p>
                </div>

                <!-- Awarded to section -->
                <div class="text-center">
                    <p class="uppercase tracking-wide text-sm sm:text-base mb-4">PROUDLY AWARDED TO</p>
                    <h2 class="text-4xl sm:text-5xl font-serif text-red-700 mb-1">{{ recipientName }}</h2>
                    <p class="text-lg mb-6">{{ role }}</p>
                </div>

                <!-- Project name -->
                <div class="text-center mb-10">
                    <h3 class="text-xl sm:text-2xl font-bold">{{ projectName }}</h3>
                </div>

                <!-- Description -->
                <div class="text-center max-w-2xl mx-auto mb-12">
                    <p class="text-base sm:text-lg">
                        This certificate is an acknowledgment from Nasscom Foundation
                        MyKartavya for your volunteering contribution.
                    </p>
                </div>

                <!-- Signature area -->
                <div class="flex justify-center items-center">
                    <div class="text-center">
                        <!-- Signature image -->
                        <div class="h-12 mb-2">
                            <svg viewBox="0 0 200 50" class="h-full w-auto">
                                <text x="20" y="30" font-family="cursive" font-size="24" fill="black">JyotiSharma</text>
                            </svg>
                        </div>
                        <div class="w-48 border-t border-gray-400 mx-auto mb-2"></div>
                        <p class="font-bold text-base sm:text-lg">{{ signatoryName }}</p>
                        <p class="text-sm">{{ signatoryTitle }}</p>
                    </div>
                </div>
            </div>
        </div>
    </div>
</template>

<style scoped>
/* Additional styles to match font and other specific details */
@import url('https://fonts.googleapis.com/css2?family=Playfair+Display:wght@400;700&display=swap');

.font-serif {
    font-family: 'Playfair Display', serif;
}

/* Circuit board pattern styles for the red background */
.bg-red-700 {
    background-color: #b91c1c;
    background-image: radial-gradient(circle, rgba(255, 255, 255, 0.1) 1px, transparent 1px);
    background-size: 20px 20px;
}
</style>