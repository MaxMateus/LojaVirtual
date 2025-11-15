<template>
  <div class="relative min-h-screen bg-mist text-slate-800">
    <div class="pointer-events-none absolute inset-x-0 top-0 h-64 bg-gradient-to-b from-primary/15 via-transparent to-transparent"></div>

    <Header />

    <main class="relative max-w-7xl mx-auto px-4 sm:px-6 lg:px-8 py-10 space-y-12">
      <slot />
    </main>

    <Footer />
  </div>
</template>

<script setup>
import Header from './Header.vue'
import Footer from './Footer.vue'
</script>
