<script setup lang="ts">
  import { useHead } from 'unhead'

  definePage({
    name: 'home',
    // alias: ['home'],
    meta: {
      title: 'Home',
      navOrder: 1,
    },
  })

  useHead({
    title: 'Home',
  })
</script>
<template>
  <div>
    <HeroSection />
    <AboutTemplate />
    <WalkThrough />
  </div>
</template>
<style scoped></style>
