<script setup lang="ts">
  import { computed } from 'vue'
  import site from '~/site'
  import { useHead, useSeoMeta } from 'unhead'
  import { useRoute } from 'vue-router/auto'
  import { checkDarkTheme } from '~/composables/dark-color-scheme-check'
  import type { Script } from '@unhead/schema'
  type TurboScript = Script & { once: true }

  const { title, description, author } = site
  const route = useRoute()

  useSeoMeta({
    title,
    ogTitle: title,
    description,
    ogDescription: description,
    ogImage: 'https://example.com/image.png',
    twitterCard: 'summary_large_image',
  })

  useHead({
    title: computed(() => route.meta.title),
    titleTemplate: (titleChunk) => {
      return titleChunk ? `${titleChunk} - ${title}` : title
    },
    htmlAttrs: { lang: 'en-US' },
    meta: [
      { property: 'keywords', content: route.meta.tags?.toString() },
      { property: 'author', content: author },
      {
        property: 'twitter:image',
        content: 'https://icons.vuetelescope.com/vue.svg',
      },
      {
        property: 'twitter:image:alt',
        content: 'Vue',
      },
      {
        property: 'twitter:site',
        content: '@pinegrow',
      },
      {
        property: 'twitter:card',
        content: 'summary',
      },
    ],
    script: [{ children: checkDarkTheme, once: true } as TurboScript],
    link: [
      {
        rel: 'icon',
        type: 'image/x-icon',
        href: '/favicon.ico',
      },
    ],
  })
</script>

<template>
  <div></div>
</template>
