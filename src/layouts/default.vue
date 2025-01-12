<script setup lang="ts">
  const route = useRoute()

  const pageMeta = computed(() => {
    return {
      title: route.meta.title,
      description: route.meta.description,
      ogImage: route.meta.ogImage,
      canonicalUrl: route.meta.canonicalUrl || route.fullPath,
      generator: route.meta.generator,
      tags: route.meta.tags,
    }
  })

  useHeadAndMeta(pageMeta)
</script>

<template>
  <div>
    <div
      class="flex flex-col bg-white dark:bg-neutral-950 text-neutral-900 dark:text-neutral-50"
    >
      <!-- <NavBar class="fixed bg-white dark:bg-neutral-950 shadow z-20" /> -->
      <!-- <main class="mt-24 shadow"> -->
      <main>
        <router-view />
      </main>
      <!-- </main> -->
      <!-- <TheFooter /> -->
    </div>
  </div>
</template>
<style></style>
