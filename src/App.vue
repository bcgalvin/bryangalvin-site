<template>
  <NavBar />
  <main class="px-7 py-10">
    <router-view />
    <Footer />
  </main>
</template>

<script setup lang="ts">
import { useHead } from '@vueuse/head'

useHead({
  meta: [
    { property: 'og:title', content: 'Bryan Galvin' },
    { property: 'og:image', content: 'https://bryangalvin.com/avatar.jpg' },
    { name: 'description', content: 'Collection of Bryan Galvin\'s thoughts & feels.' },
    { name: 'twitter:card', content: 'summary' },
    { name: 'twitter:creator', content: '@bryan_galvin' },
  ],
})
</script>