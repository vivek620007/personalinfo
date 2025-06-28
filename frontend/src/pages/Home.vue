<!-- <template>
  <div class="max-w-3xl py-12 mx-auto">
    <h2 class="font-bold text-lg text-gray-600 mb-4">
      Welcome {{ session.user }}!
    </h2>

    <Button theme="gray" variant="solid" icon-left="code" @click="ping.fetch" :loading="ping.loading">
      Click to send 'ping' request
    </Button>
    <div>
      {{ ping.data }}
    </div>
    <pre>{{ ping }}</pre>

    <div class="flex flex-row space-x-2 mt-4">
      <Button @click="showDialog = true">Open Dialog</Button>
      <Button @click="session.logout.submit()">Logout</Button>
    </div>

    <Dialog title="Title" v-model="showDialog"> Dialog content </Dialog>
  </div>
</template>

<script setup>
import { ref } from 'vue'
import { Dialog } from 'frappe-ui'
import { createResource } from 'frappe-ui'
import { session } from '../data/session'

const ping = createResource({
  url: 'ping',
  auto: true,
})

const showDialog = ref(false)
</script> -->


<!-- <template>
  <Navbar />
  <div class="flex flex-col md:flex-row items-center justify-center bg-gray-900 text-white h-[500px] p-6">
   
    <div class="relative">
      <div class="absolute inset-0 flex justify-center items-center">
        <div class="w-60 h-60 bg-gray-800 rounded-xl transform -rotate-45"></div>
      </div>
      <img src="" alt="" class="relative z-10 w-60 h-60 md:w-80 md:h-80 rounded-full object-cover" />
    </div>
    
    <div class="text-center md:text-left mt-6 md:mt-0 md:ml-10">
      <p class="text-cyan-400 text-lg font-medium">Hi I am </p>
      <h1 class="text-3xl md:text-5xl font-bold mt-2">Vivek Kumar</h1>
      <p class="text-gray-400 text-lg font-medium mt-2">Frontend Developer & UX/UI Designer</p>
      <div class="flex justify-center md:justify-start items-center gap-4 mt-4">
        <a href="https://github.com" target="_blank" class="text-gray-400 hover:text-cyan-400">
          <svg class="w-8 h-8" xmlns="http://www.w3.org/2000/svg" fill="currentColor" viewBox="0 0 24 24">
            <path
              d="M12 .5C5.74.5.5 5.74.5 12c0 5.1 3.29 9.42 7.85 10.96.57.1.78-.25.78-.55 0-.27-.01-1.16-.01-2.1-3.19.68-3.87-1.38-3.87-1.38-.52-1.34-1.28-1.69-1.28-1.69-1.05-.72.08-.7.08-.7 1.16.08 1.77 1.19 1.77 1.19 1.03 1.76 2.71 1.25 3.37.96.1-.75.4-1.25.73-1.54-2.54-.29-5.22-1.27-5.22-5.66 0-1.25.45-2.27 1.19-3.07-.12-.3-.52-1.52.12-3.18 0 0 .97-.31 3.18 1.18.92-.25 1.91-.37 2.89-.37.98 0 1.97.12 2.89.37 2.21-1.49 3.18-1.18 3.18-1.18.64 1.66.24 2.88.12 3.18.74.8 1.19 1.82 1.19 3.07 0 4.4-2.68 5.37-5.23 5.66.41.36.77 1.08.77 2.17 0 1.57-.01 2.84-.01 3.22 0 .3.21.65.79.54 4.56-1.54 7.84-5.86 7.84-10.96C23.5 5.74 18.26.5 12 .5z" />
          </svg>
        </a>
        <a href="https://linkedin.com" target="_blank" class="text-gray-400 hover:text-cyan-400">
          <svg class="w-8 h-8" xmlns="http://www.w3.org/2000/svg" fill="currentColor" viewBox="0 0 24 24">
            <path
              d="M19.8 3H4.2C3.08 3 2.2 3.88 2.2 5v14c0 1.12.88 2 2 2h15.6c1.12 0 2-.88 2-2V5c0-1.12-.88-2-2-2zM8.75 18.5H6.25v-9h2.5v9zm-1.25-9.95c-.83 0-1.5-.67-1.5-1.5S6.67 6.5 7.5 6.5 9 7.17 9 8s-.67 1.55-1.5 1.55zm11.5 9.95h-2.5v-4.5c0-1.1-.9-2-2-2s-2 .9-2 2v4.5H10.75v-9h2.5v1.15c.67-.45 1.5-.65 2.25-.65 2.5 0 3.5 2.25 3.5 4.25v4.25z" />
          </svg>
        </a>
      </div>
    </div>
  </div>
</template>

<script setup>
import Navbar from '../components/Navbar.vue';
</script> -->


<template>
  <Navbar />
  <div class="min-h-screen bg-[#04152D] text-white flex flex-col justify-center p-4">
    <div class="container mx-auto max-w-6xl flex flex-col-reverse md:flex-row items-center">
      <!-- Text Content -->
      <div class="w-full md:w-1/2 pr-0 md:pr-12 text-center md:text-left">
        <h2 class="text-lg mb-2">Hi I am</h2>
        <h1 class="text-4xl font-bold mb-4">Vivek Kumar</h1>
        <div class="text-2xl text-orange-500 mb-6">UI/UX designer</div>
        <!-- Stats -->
        <div class="flex justify-center md:justify-start items-center gap-4 mt-4">
          <a href="https://github.com" target="_blank" class="text-gray-400 hover:text-orange-500">
            <svg class="w-8 h-8" xmlns="http://www.w3.org/2000/svg" fill="currentColor" viewBox="0 0 24 24">
              <path
                d="M12 .5C5.74.5.5 5.74.5 12c0 5.1 3.29 9.42 7.85 10.96.57.1.78-.25.78-.55 0-.27-.01-1.16-.01-2.1-3.19.68-3.87-1.38-3.87-1.38-.52-1.34-1.28-1.69-1.28-1.69-1.05-.72.08-.7.08-.7 1.16.08 1.77 1.19 1.77 1.19 1.03 1.76 2.71 1.25 3.37.96.1-.75.4-1.25.73-1.54-2.54-.29-5.22-1.27-5.22-5.66 0-1.25.45-2.27 1.19-3.07-.12-.3-.52-1.52.12-3.18 0 0 .97-.31 3.18 1.18.92-.25 1.91-.37 2.89-.37.98 0 1.97.12 2.89.37 2.21-1.49 3.18-1.18 3.18-1.18.64 1.66.24 2.88.12 3.18.74.8 1.19 1.82 1.19 3.07 0 4.4-2.68 5.37-5.23 5.66.41.36.77 1.08.77 2.17 0 1.57-.01 2.84-.01 3.22 0 .3.21.65.79.54 4.56-1.54 7.84-5.86 7.84-10.96C23.5 5.74 18.26.5 12 .5z" />
            </svg>
          </a>
          <a href="https://linkedin.com" target="_blank" class="text-gray-400 hover:text-orange-500">
            <svg class="w-8 h-8" xmlns="http://www.w3.org/2000/svg" fill="currentColor" viewBox="0 0 24 24">
              <path
                d="M19.8 3H4.2C3.08 3 2.2 3.88 2.2 5v14c0 1.12.88 2 2 2h15.6c1.12 0 2-.88 2-2V5c0-1.12-.88-2-2-2zM8.75 18.5H6.25v-9h2.5v9zm-1.25-9.95c-.83 0-1.5-.67-1.5-1.5S6.67 6.5 7.5 6.5 9 7.17 9 8s-.67 1.55-1.5 1.55zm11.5 9.95h-2.5v-4.5c0-1.1-.9-2-2-2s-2 .9-2 2v4.5H10.75v-9h2.5v1.15c.67-.45 1.5-.65 2.25-.65 2.5 0 3.5 2.25 3.5 4.25v4.25z" />
            </svg>
          </a>
        </div>

        <div class="mt-12 grid grid-cols-3 gap-4 bg-gray-900 p-4 rounded-lg">
          <div class="text-center">
            <div class="text-2xl font-bold text-orange-500">5+</div>
            <div class="text-sm">Experiences</div>
          </div>
          <div class="text-center">
            <div class="text-2xl font-bold text-orange-500">20+</div>
            <div class="text-sm">Project done</div>
          </div>
          <div class="text-center">
            <div class="text-2xl font-bold text-orange-500">80+</div>
            <div class="text-sm">Happy Clients</div>
          </div>
        </div>
      </div>




      <!-- Image Container -->
      <div class="w-full md:w-1/2 mb-8 md:mb-0 relative">
        <div class="relative z-10">
          <!-- <img src="" alt="" class="mx-auto rounded-full shadow-lg object-cover h-[500px] w-full" /> -->
          <img src="https://res.cloudinary.com/deuh2cmub/image/upload/v1745842835/Vivek_a4cbqt.jpg" alt=""
            class="mx-auto rounded-full shadow-lg object-cover h-[500px] w-full" />
        </div>
        <div class="absolute inset-0 bg-gradient-to-r from-transparent to-[#04152D] opacity-50 z-0"></div>
      </div>
    </div>
  </div>
  <About />
  <Skill />
  <Contact />
  <Project />

</template>

<script setup>
import Navbar from '../components/Navbar.vue';
import Footer from '../components/Footer.vue';
import About from './About.vue';
import Skill from './Skill.vue';
import Contact from './Contact.vue';
import Project from './Project.vue';
</script>

<style scoped>
/* Additional custom styles can be added here if needed */
</style>
