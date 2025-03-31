<template>
  <section id="about" class="py-20">
    <div class="max-w-7xl mx-auto px-4 sm:px-6 lg:px-8">
      <div class="text-center mb-16">
        <h2 class="text-3xl font-bold text-gray-900">About Me</h2>
        <div class="w-16 h-1 bg-indigo-600 mx-auto mt-4 mb-6"></div>
        <p class="text-gray-600 max-w-2xl mx-auto">Get to know me better</p>
      </div>
      <div class="flex flex-col md:flex-row items-center">
        <div class="md:w-1/2 mb-10 md:mb-0 md:pr-10">
          <h3 class="text-2xl font-bold text-gray-900 mb-4">Who am I?</h3>
          <p class="text-gray-600 mb-4">
            저는 아름답고 기능적이며 사용자 친화적인 웹사이트 제작에 열정을 가진 웹 개발자입니다. 여러 해의 경험을 통해 소규모 비즈니스 사이트부터 복잡한 웹 애플리케이션까지 다양한 프로젝트를 진행해왔습니다.
          </p>
          <p class="text-gray-600 mb-6">
            코딩하지 않을 때에는 새로운 기술을 탐구하고, 오픈 소스 프로젝트에 기여하며, 야외 활동을 즐깁니다.
          </p>
          <div class="flex space-x-4">
            <a href="#" class="text-indigo-600 hover:text-indigo-800 transition-colors">
              <GithubIcon class="h-6 w-6" />
            </a>
            <a href="#" class="text-indigo-600 hover:text-indigo-800 transition-colors">
              <LinkedinIcon class="h-6 w-6" />
            </a>
            <a href="#" class="text-indigo-600 hover:text-indigo-800 transition-colors">
              <TwitterIcon class="h-6 w-6" />
            </a>
          </div>
        </div>
        <div class="md:w-1/2">
          <div class="grid grid-cols-2 gap-4">
            <div class="bg-white p-6 rounded-lg shadow-md">
              <CodeIcon class="h-10 w-10 text-indigo-600 mb-4" />
              <h4 class="text-xl font-bold text-gray-900 mb-2">웹 개발</h4>
              <p class="text-gray-600">반응형 및 동적인 웹 애플리케이션 개발</p>
            </div>
            <div class="bg-white p-6 rounded-lg shadow-md">
              <PaletteIcon class="h-10 w-10 text-indigo-600 mb-4" />
              <h4 class="text-xl font-bold text-gray-900 mb-2">UI/UX 디자인</h4>
              <p class="text-gray-600">직관적이고 아름다운 사용자 인터페이스 디자인</p>
            </div>
            <div class="bg-white p-6 rounded-lg shadow-md">
              <ServerIcon class="h-10 w-10 text-indigo-600 mb-4" />
              <h4 class="text-xl font-bold text-gray-900 mb-2">백엔드 개발</h4>
              <p class="text-gray-600">견고한 서버 사이드 애플리케이션 구축</p>
            </div>
            <div class="bg-white p-6 rounded-lg shadow-md">
              <TrendingUpIcon class="h-10 w-10 text-indigo-600 mb-4" />
              <h4 class="text-xl font-bold text-gray-900 mb-2">SEO 최적화</h4>
              <p class="text-gray-600">검색 엔진에서 웹사이트 가시성 향상</p>
            </div>
          </div>
        </div>
      </div>
    </div>
  </section>
</template>

<script setup>
import { GithubIcon, LinkedinIcon, TwitterIcon, CodeIcon, PaletteIcon, ServerIcon, TrendingUpIcon } from 'lucide-vue-next';
</script>