<template>
  <transition name="fade">
    <div v-if="show" class="fixed inset-0 z-50 flex items-center justify-center">
      <!-- Modal backdrop -->
      <div class="fixed inset-0 bg-black opacity-50" @click="closeModal"></div>
      <!-- Modal content -->
      <div class="bg-white p-6 rounded-lg shadow-lg z-10 max-w-lg w-full mx-4">
        <h3 class="text-2xl font-bold mb-4">{{ title }}</h3>
        <slot></slot>
        <button class="bg-indigo-600 text-white px-4 py-2 rounded mt-4" @click="closeModal">Close</button>
      </div>
    </div>
  </transition>
</template>

<script setup>
import { defineProps, defineEmits } from 'vue';

const props = defineProps({
  show: { type: Boolean, required: true },
  title: { type: String, required: true }
});

const emit = defineEmits(['close']);

const closeModal = () => {
  emit('close');
};
</script>

<style scoped>
.fade-enter-active, .fade-leave-active {
  transition: opacity 0.5s;
}
.fade-enter-from, .fade-leave-to {
  opacity: 0;
}
</style>