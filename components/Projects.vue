<template>
  <section id="projects" class="py-20">
    <div class="max-w-7xl mx-auto px-4 sm:px-6 lg:px-8">
      <div class="text-center mb-16">
        <h2 class="text-3xl font-bold text-gray-900">My Projects</h2>
        <div class="w-16 h-1 bg-indigo-600 mx-auto mt-4 mb-6"></div>
        <p class="text-gray-600 max-w-2xl mx-auto">Check out some of my recent work</p>
      </div>
      <div class="grid md:grid-cols-2 lg:grid-cols-3 gap-8">
        <!-- 프로젝트 1 카드 -->
        <div class="bg-white rounded-lg overflow-hidden shadow-md cursor-pointer" @click="activeModalIndex = 1">
          <div class="h-48 overflow-hidden">
            <img src="/assets/images/placeholder.png?height=300&width=500" alt="Project 1" class="w-full h-full object-cover transition-transform duration-300 hover:scale-110\" />
          </div>
          <div class="p-6">
            <h4 class="text-xl font-bold text-gray-900 mb-2\">Project 1</h4>
            <p class="text-gray-600 mb-4\">A fully responsive e-commerce platform built with Vue.js and Node.js.</p>
            <div class="flex flex-wrap gap-2 mb-4">
              <span class="px-3 py-1 bg-indigo-100 text-indigo-800 rounded-full text-sm">Vue.js</span>
              <span class="px-3 py-1 bg-indigo-100 text-indigo-800 rounded-full text-sm">Node.js</span>
              <span class="px-3 py-1 bg-indigo-100 text-indigo-800 rounded-full text-sm">MongoDB</span>
            </div>
            <div class="flex space-x-4">
              <a href="#" class="text-indigo-600 hover:text-indigo-800 transition-colors">
                <ExternalLinkIcon class="h-5 w-5" />
              </a>
              <a href="#" class="text-indigo-600 hover:text-indigo-800 transition-colors">
                <GithubIcon class="h-5 w-5" />
              </a>
            </div>
          </div>
        </div>
        <!-- 프로젝트 2 카드 -->
        <div class="bg-white rounded-lg overflow-hidden shadow-md cursor-pointer" @click="activeModalIndex = 3">
          <div class="h-48 overflow-hidden">
            <img src="/assets/images/placeholder.png?height=300&width=500" alt="Project 2" class="w-full h-full object-cover transition-transform duration-300 hover:scale-110\" />
          </div>
          <div class="p-6">
            <h4 class="text-xl font-bold text-gray-900 mb-2\">Project 2</h4>
            <p class="text-gray-600 mb-4\">A fully responsive e-commerce platform built with Vue.js and Node.js.</p>
            <div class="flex flex-wrap gap-2 mb-4">
              <span class="px-3 py-1 bg-indigo-100 text-indigo-800 rounded-full text-sm">JAVA</span>
              <span class="px-3 py-1 bg-indigo-100 text-indigo-800 rounded-full text-sm">JPA</span>
              <span class="px-3 py-1 bg-indigo-100 text-indigo-800 rounded-full text-sm">Spring Boot</span>
              <span class="px-3 py-1 bg-indigo-100 text-indigo-800 rounded-full text-sm">MySQL</span>
            </div>
            <div class="flex space-x-4">
              <a href="#" class="text-indigo-600 hover:text-indigo-800 transition-colors">
                <ExternalLinkIcon class="h-5 w-5" />
              </a>
              <a href="#" class="text-indigo-600 hover:text-indigo-800 transition-colors">
                <GithubIcon class="h-5 w-5" />
              </a>
            </div>
          </div>
        </div>

      <!-- 프로젝트 3 카드 -->
      <div class="bg-white rounded-lg overflow-hidden shadow-md cursor-pointer" @click="activeModalIndex = 2">
          <div class="h-48 overflow-hidden">
            <img src="/assets/images/placeholder.png?height=300&width=500" alt="Project 3" class="w-full h-full object-cover transition-transform duration-300 hover:scale-110\" />
          </div>
          <div class="p-6">
            <h4 class="text-xl font-bold text-gray-900 mb-2\">Project 3</h4>
            <p class="text-gray-600 mb-4\">A fully responsive e-commerce platform built with Vue.js and Node.js.</p>
            <div class="flex flex-wrap gap-2 mb-4">
              <span class="px-3 py-1 bg-indigo-100 text-indigo-800 rounded-full text-sm">Node.js</span>
              <span class="px-3 py-1 bg-indigo-100 text-indigo-800 rounded-full text-sm">AWS CDK</span>
              <span class="px-3 py-1 bg-indigo-100 text-indigo-800 rounded-full text-sm">AWS RDS</span>
            </div>
            <div class="flex space-x-4">
              <a href="#" class="text-indigo-600 hover:text-indigo-800 transition-colors">
                <ExternalLinkIcon class="h-5 w-5" />
              </a>
              <a href="#" class="text-indigo-600 hover:text-indigo-800 transition-colors">
                <GithubIcon class="h-5 w-5" />
              </a>
            </div>
          </div>
        </div>
      </div>
      <div class="text-center mt-12">
        <a href="#" class="inline-flex items-center text-indigo-600 hover:text-indigo-800 transition-colors">
          View All Projects
          <ArrowRightIcon class="h-5 w-5 ml-2" />
        </a>
      </div>
    </div>

    <!-- Modal for Project 1 -->
    <transition name="fade">
      <div v-if="activeModalIndex === 1" class="fixed inset-0 z-50 flex items-center justify-center">
        <!-- Modal backdrop -->
        <div class="fixed inset-0 bg-black opacity-50" @click="activeModalIndex = null"></div>
        <!-- Modal content -->
        <div class="bg-white p-6 rounded-lg shadow-lg z-10 max-w-lg w-full mx-4">
          <h3 class="text-2xl font-bold mb-4">Project 1 Details</h3>
          <div>
            <h4 class="font-semibold">1. 개요</h4>
            <p class="mb-2">프로젝트의 개요를 여기에 작성하세요. (예: 이 프로젝트는 ~)</p>
            <h4 class="font-semibold">2. 성과</h4>
            <p class="mb-2">프로젝트의 주요 성과를 여기에 작성하세요. (예: 사용자 증가, 매출 상승 등)</p>
            <h4 class="font-semibold">3. 사용 스킬</h4>
            <p>프로젝트에 사용된 기술 스택을 여기에 작성하세요. (예: Vue.js, Node.js, MongoDB 등)</p>
          </div>
          <button class="bg-indigo-600 text-white px-4 py-2 rounded" @click="activeModalIndex = null">Close</button>
        </div>
      </div>
    </transition>

    <!-- Modal for Project 2 -->
    <transition name="fade">
      <div v-if="activeModalIndex === 2" class="fixed inset-0 z-50 flex items-center justify-center">
        <!-- Modal backdrop -->
        <div class="fixed inset-0 bg-black opacity-50" @click="activeModalIndex = null"></div>
        <!-- Modal content -->
        <div class="bg-white p-6 rounded-lg shadow-lg z-10 max-w-lg w-full mx-4">
          <h3 class="text-2xl font-bold mb-4">Project 2 Details</h3>
          <div>
            <h4 class="font-semibold">1. 개요</h4>
            <p class="mb-2">프로젝트의 개요를 여기에 작성하세요. (예: 이 프로젝트는 ~)</p>
            <h4 class="font-semibold">2. 성과</h4>
            <p class="mb-2">프로젝트의 주요 성과를 여기에 작성하세요. (예: 사용자 증가, 매출 상승 등)</p>
            <h4 class="font-semibold">3. 사용 스킬</h4>
            <p>프로젝트에 사용된 기술 스택을 여기에 작성하세요. (예: Vue.js, Node.js, MongoDB 등)</p>
          </div>
          <button class="bg-indigo-600 text-white px-4 py-2 rounded" @click="activeModalIndex = null">Close</button>
        </div>
      </div>
    </transition>

    <!-- Modal for Project 3 -->
    <transition name="fade">
      <div v-if="activeModalIndex === 3" class="fixed inset-0 z-50 flex items-center justify-center">
        <!-- Modal backdrop -->
        <div class="fixed inset-0 bg-black opacity-50" @click="activeModalIndex = null"></div>
        <!-- Modal content -->
        <div class="bg-white p-6 rounded-lg shadow-lg z-10 max-w-lg w-full mx-4">
          <h3 class="text-2xl font-bold mb-4">Project 3 Details</h3>
          <div>
            <h4 class="font-semibold">1. 개요</h4>
            <p class="mb-2">프로젝트의 개요를 여기에 작성하세요. (예: 이 프로젝트는 ~)</p>
            <h4 class="font-semibold">2. 성과</h4>
            <p class="mb-2">프로젝트의 주요 성과를 여기에 작성하세요. (예: 사용자 증가, 매출 상승 등)</p>
            <h4 class="font-semibold">3. 사용 스킬</h4>
            <p>프로젝트에 사용된 기술 스택을 여기에 작성하세요. (예: Vue.js, Node.js, MongoDB 등)</p>
          </div>
          <button class="bg-indigo-600 text-white px-4 py-2 rounded" @click="activeModalIndex = null">Close</button>
        </div>
      </div>
    </transition>
  </section>
</template>

<script setup>
import { ref } from 'vue';
import { ExternalLinkIcon, GithubIcon, ArrowRightIcon } from 'lucide-vue-next';

const activeModalIndex = ref(null);
</script>

<style>
/* 모달 트랜지션 효과 */
.fade-enter-active, .fade-leave-active {
  transition: opacity 0.5s;
}
.fade-enter-from, .fade-leave-to {
  opacity: 0;
}
</style>