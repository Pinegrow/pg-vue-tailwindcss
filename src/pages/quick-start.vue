<script setup lang="ts">
  import { useHead } from 'unhead'
  import QuickStart from '~/content/index.md'

  definePage({
    name: 'quick-start',
    meta: {
      title: 'Quick Start',
      navOrder: 2,
    },
  })

  useHead({
    title: 'Quick Start',
  })
</script>
<template>
  <div class="pb-12">
    <TheHeader>
      <div>
        <div class="flex items-center">
          <h2 class="text-5xl">Quick Start</h2>
        </div>
        <div class="flex items-center mt-2">
          <h6 class="mt-2">Github repo for this template</h6>
          <BaseButton
            size="xs"
            class="ml-2 pg-primary-container-text"
            color="gray"
            to="https://github.com/pinegrow/pg-vue-tailwindcss"
            target="_blank"
          >
            <span>Click here</span>
          </BaseButton>
        </div>
      </div>
    </TheHeader>
    <section>
      <div class="container mx-auto px-10 w-full">
        <div class="flex flex-col rounded-lg">
          <article
            class="dark:xl:divide-gray-700 xl:divide-gray-200 xl:divide-y"
          >
            <div
              class="dark:divide-gray-700 divide-gray-200 divide-y pb-16 xl:divide-y-0 xl:gap-x-10 xl:grid xl:grid-cols-4 xl:pb-20 xl:sticky"
              style="grid-template-rows: auto 1fr"
            >
              <div
                class="dark:divide-gray-700 divide-gray-200 divide-y xl:col-span-3 xl:pb-0 xl:row-span-2"
              >
                <div
                  id="post"
                  class="dark:prose-invert dark:prose-gray-100 flex flex-col heading-offset max-w-none prose prose-gray-800 rounded-lg"
                >
                  <QuickStart />
                </div>
              </div>
            </div>
          </article>
        </div>
      </div>
    </section>
  </div>
</template>
<style scoped></style>
