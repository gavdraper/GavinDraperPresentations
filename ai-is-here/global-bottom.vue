<!-- global-bottom.vue -->
<template>
  <footer class="fixed bottom-0 left-0 right-0 px-8 py-3 bg-gradient-to-r from-slate-900/90 to-slate-800/90 backdrop-blur-sm text-white z-50">
    <div class="flex items-center justify-between max-w-6xl mx-auto">
      <div class="flex items-center space-x-6">
        <div class="text-xs text-slate-300">gavin.draper@outlook.com</div>
        <div class="text-xs text-slate-400">|</div>
        <div class="text-xs text-slate-300">@gavdraper</div>
      </div>
      

    </div>
  </footer>
</template>

<script setup>
import { computed } from 'vue'
import { useNav } from '@slidev/client'

const { currentPage, total } = useNav()
const currentSlide = computed(() => currentPage.value)
const totalSlides = computed(() => total.value)
</script>

<style scoped>
footer {
  border-top: 2px solid rgba(14, 165, 233, 0.4);
  backdrop-filter: blur(12px);
  box-shadow: 0 -4px 20px rgba(0, 0, 0, 0.3);
}
</style>
