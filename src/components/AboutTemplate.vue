<script setup lang="ts">
  import site from '~/site'
  const { description } = site
</script>

<template>
  <div class="container mx-auto px-4 py-24 relative">
    <div class="flex flex-wrap items-center justify-center">
      <div
        class="mx-auto p-4 rounded-2xl w-full sm:w-4/5 lg:w-5/12 pg-primary-container pg-on-primary-container-text"
      >
        <div class="flex flex-wrap justify-between sm:flex-nowrap">
          <div class="p-5 text-center w-full whitespace-nowrap">
            <h5>Meta-framework</h5>
            <p class="pg-primary-text">Vite-powered</p>
          </div>
          <div
            class="hidden items-center justify-center my-4 relative w-1 sm:flex"
          >
            <span
              class="-ml-px absolute h-full w-0.5 pg-surface-container"
              aria-hidden="true"
            />
          </div>
          <div
            class="flex h-2 items-center justify-center my-4 relative w-full sm:hidden"
          >
            <span
              class="-ml-px absolute w-full h-0.5 pg-surface-container"
              aria-hidden="true"
            />
          </div>
          <div class="p-5 text-center w-full whitespace-nowrap">
            <h5>UI-framework</h5>
            <p class="pg-primary-text">Tailwind CSS</p>
          </div>
        </div>
      </div>
      <div
        class="mt-4 mx-auto px-2 py-4 text-center w-full sm:w-4/5 lg:mt-0 lg:text-left lg:w-5/12"
      >
        <h3 class="capitalize mb-2">About This Template</h3>
        <h6 class="capitalize mb-2 pg-primary-text">{{ description }}</h6>
        <p class="mb-6 pt-3">
          This is a starter template that pre-includes the
          <a
            class="font-mono text-sm underline pg-primary-text"
            target="_blank"
            external
            href="https://www.npmjs.com/package/@pinegrow/vite-plugin"
            >Pinegrow Vite Plugin</a
          >
          <span>, </span>
          <a
            class="font-mono text-sm underline pg-primary-text"
            target="_blank"
            external
            href="https://www.npmjs.com/package/@pinegrow/tailwindcss-plugin"
            >Pinegrow Tailwind CSS Plugin</a
          >
          that enables you to visually design your Vue single-file components in
          Vue Designer.
        </p>
        <div class="flex justify-center lg:justify-start">
          <BaseButton
            label="Quick Start >"
            size="lg"
            to="/quick-start"
          ></BaseButton>
        </div>
      </div>
    </div>
  </div>
</template>
<style scoped></style>
