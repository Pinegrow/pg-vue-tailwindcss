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
  <main>A Fresh Start!</main>
</template>
<style scoped></style>
