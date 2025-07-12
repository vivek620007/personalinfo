<script setup>
import { ref } from 'vue';

// Project data
const projects = ref([
    {
        id: 1,
        title: 'E-commerce Platform',
        description: 'A fully responsive e-commerce website with product filtering, cart functionality, and payment integration.',
        image: '/images/image.png',
        technologies: ['React', 'Redux', 'Node.js', 'MongoDB'],
        liveDemo: '#',
        sourceCode: '#'
    },
    {
        id: 2,
        title: 'Task Management App',
        description: 'A drag-and-drop task management application with user authentication and real-time updates.',
        image: '/images/image copy.png',
        technologies: ['React', 'Firebase', 'Tailwind CSS'],
        liveDemo: '#',
        sourceCode: '#'
    },
    {
        id: 3,
        title: 'Weather Dashboard',
        description: 'A weather application that displays current conditions and forecasts based on user location or search.',
        image: '/images/image copy 2.png',
        technologies: ['React', 'API Integration', 'CSS'],
        liveDemo: '#',
        sourceCode: '#'
    }
]);
</script>

<template>
    <div class="min-h-screen max-w-4xl mx-auto px-4 py-8 pt-32">
        <div class="max-w-6xl mx-auto">
            <h1 class="text-[28px] font-bold text-center mb-12">My Projects</h1>

            <div class="grid grid-cols-1 md:grid-cols-2 lg:grid-cols-3 gap-6">
                <!-- Project Cards -->
                <div v-for="project in projects" :key="project.id"
                    class="bg-white rounded-lg overflow-hidden shadow-md flex flex-col transition-transform duration-300 hover:shadow-lg">
                    <img :src="project.image" :alt="project.title" class="w-full h-48 object-cover" />
                    <div class="p-6 flex-grow">
                        <h3 class="text-xl font-semibold mb-2 text-gray-900">{{ project.title }}</h3>
                        <p class="text-gray-600 mb-4">{{ project.description }}</p>

                        <div class="flex flex-wrap gap-2 mb-6">
                            <span v-for="(tech, index) in project.technologies" :key="index"
                                class="bg-purple-100 text-purple-700 px-3 py-1 text-sm rounded-md">
                                {{ tech }}
                            </span>
                        </div>

                        <div class="flex items-center gap-4 mt-auto">
                            <a :href="project.liveDemo"
                                class="inline-flex items-center text-purple-700 hover:text-purple-900">
                                <svg xmlns="http://www.w3.org/2000/svg" class="h-5 w-5 mr-1" viewBox="0 0 20 20"
                                    fill="currentColor">
                                    <path fill-rule="evenodd"
                                        d="M10 18a8 8 0 100-16 8 8 0 000 16zM9.555 7.168A1 1 0 008 8v4a1 1 0 001.555.832l3-2a1 1 0 000-1.664l-3-2z"
                                        clip-rule="evenodd" />
                                </svg>
                                Live Demo
                            </a>
                            <a :href="project.sourceCode"
                                class="inline-flex items-center text-gray-700 hover:text-gray-900">
                                <svg xmlns="http://www.w3.org/2000/svg" class="h-5 w-5 mr-1" viewBox="0 0 20 20"
                                    fill="currentColor">
                                    <path fill-rule="evenodd"
                                        d="M12.316 3.051a1 1 0 01.633 1.265l-4 12a1 1 0 11-1.898-.632l4-12a1 1 0 011.265-.633zM5.707 6.293a1 1 0 010 1.414L3.414 10l2.293 2.293a1 1 0 11-1.414 1.414l-3-3a1 1 0 010-1.414l3-3a1 1 0 011.414 0zm8.586 0a1 1 0 011.414 0l3 3a1 1 0 010 1.414l-3 3a1 1 0 11-1.414-1.414L16.586 10l-2.293-2.293a1 1 0 010-1.414z"
                                        clip-rule="evenodd" />
                                </svg>
                                Source Code
                            </a>
                        </div>
                    </div>
                </div>
            </div>
        </div>
    </div>
</template>

<style scoped>
/* Additional custom styles can be added here if needed */
</style>