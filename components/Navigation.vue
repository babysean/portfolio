<template>
  <nav class="bg-white shadow-sm">
    <div class="max-w-7xl mx-auto px-4 sm:px-6 lg:px-8">
      <div class="flex justify-between h-16">
        <div class="flex items-center">
          <span class="text-xl font-bold text-gray-900">Portfolio</span>
        </div>
        <div class="hidden md:flex items-center space-x-8">
          <a href="#home" class="text-gray-900 hover:text-primary transition-colors">Home</a>
          <a href="#about" class="text-gray-600 hover:text-primary transition-colors">About</a>
          <a href="#skills" class="text-gray-600 hover:text-primary transition-colors">Skills</a>
          <a href="#projects" class="text-gray-600 hover:text-primary transition-colors">Projects</a>
          <a href="#contact" class="text-gray-600 hover:text-primary transition-colors">Contact</a>
        </div>
        <div class="flex md:hidden items-center">
          <button @click="mobileMenuOpen = !mobileMenuOpen" class="text-gray-600">
            <MenuIcon v-if="!mobileMenuOpen" class="h-6 w-6" />
            <XIcon v-else class="h-6 w-6" />
          </button>
        </div>
      </div>
    </div>
    <!-- 모바일 메뉴 -->
    <div v-if="mobileMenuOpen" class="md:hidden">
      <div class="pt-2 pb-3 space-y-1">
        <a href="#home" @click="mobileMenuOpen = false" class="block pl-3 pr-4 py-2 text-base font-medium text-gray-900 hover:bg-gray-100">Home</a>
        <a href="#about" @click="mobileMenuOpen = false" class="block pl-3 pr-4 py-2 text-base font-medium text-gray-600 hover:bg-gray-100">About</a>
        <a href="#skills" @click="mobileMenuOpen = false" class="block pl-3 pr-4 py-2 text-base font-medium text-gray-600 hover:bg-gray-100">Skills</a>
        <a href="#projects" @click="mobileMenuOpen = false" class="block pl-3 pr-4 py-2 text-base font-medium text-gray-600 hover:bg-gray-100">Projects</a>
        <a href="#contact" @click="mobileMenuOpen = false" class="block pl-3 pr-4 py-2 text-base font-medium text-gray-600 hover:bg-gray-100">Contact</a>
      </div>
    </div>
  </nav>
</template>

<script setup>
import { ref } from 'vue';
import { Menu as MenuIcon, X as XIcon } from 'lucide-vue-next';

const mobileMenuOpen = ref(false);
</script>