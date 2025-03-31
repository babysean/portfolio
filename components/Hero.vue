<template>
  <section id="home" class="py-20 bg-gradient-to-r from-purple-600 to-indigo-600 text-white">
    <div class="max-w-7xl mx-auto px-4 sm:px-6 lg:px-8">
      <div class="flex flex-col md:flex-row items-center">
        <div class="md:w-1/2 mb-10 md:mb-0">
          <h1 class="text-4xl md:text-5xl font-bold mb-4">안녕하세요! 👋</h1>
          <h2 class="text-3xl md:text-4xl font-bold mb-6">저는 <span class="text-yellow-300">훈이코딩</span>입니다.</h2>
          <p class="text-xl mb-8">Web Developer & Backend Developer</p>
          <div class="flex space-x-4">
            <a href="#contact" class="bg-white text-indigo-600 px-6 py-3 rounded-lg font-medium hover:bg-gray-100 transition-colors">Contact Me</a>
            <a href="#projects" class="border border-white text-white px-6 py-3 rounded-lg font-medium hover:bg-white hover:text-indigo-600 transition-colors">View Work</a>
          </div>
        </div>
        <div class="md:w-1/2 flex justify-center">
          <div class="w-64 h-64 rounded-full overflow-hidden border-4 border-white shadow-lg">
            <img src="/assets/images/placeholder.png?height=256&width=256" alt="Profile" class="w-full h-full object-cover" />
          </div>
        </div>
      </div>
    </div>
  </section>
</template>