<template>
  <footer class="bg-gray-900 text-white py-12">
    <div class="max-w-7xl mx-auto px-4 sm:px-6 lg:px-8">
      <div class="flex flex-col md:flex-row justify-between items-center">
        <div class="mb-6 md:mb-0">
          <span class="text-2xl font-bold">Portfolio</span>
          <p class="mt-2 text-gray-400">Building amazing web experiences</p>
        </div>
        <div class="flex flex-col items-center md:items-end">
          <div class="flex space-x-4 mb-4">
            <a href="#" class="text-gray-400 hover:text-white transition-colors">
              <GithubIcon class="h-5 w-5" />
            </a>
            <a href="#" class="text-gray-400 hover:text-white transition-colors">
              <LinkedinIcon class="h-5 w-5" />
            </a>
            <a href="#" class="text-gray-400 hover:text-white transition-colors">
              <TwitterIcon class="h-5 w-5" />
            </a>
            <a href="#" class="text-gray-400 hover:text-white transition-colors">
              <InstagramIcon class="h-5 w-5" />
            </a>
          </div>
          <p class="text-gray-400">&copy; {{ new Date().getFullYear() }} 훈이코딩. All rights reserved.</p>
        </div>
      </div>
    </div>
  </footer>
</template>

<script setup>
import { GithubIcon, LinkedinIcon, TwitterIcon, InstagramIcon } from 'lucide-vue-next';
</script>
