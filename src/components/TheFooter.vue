<script setup lang="ts">
  // const props = defineProps({
  // 	name: {
  // 		type: String,
  // 		default: 'TheFooter',
  // 	},
  // })
</script>
<template>
  <div class="pb-24 pt-12">
    <div class="container mx-auto px-8">
      <div class="flex flex-wrap justify-center space-x-8">
        <a
          href="https://www.facebook.com/pinegrow/"
          aria-label="facebook"
          external
          target="_blank"
        >
          <BaseIcon name="i-logos-facebook"></BaseIcon>
        </a>
        <a
          href="https://twitter.com/pinegrow"
          aria-label="facebook"
          external
          target="_blank"
        >
          <BaseIcon name="i-logos-twitter"></BaseIcon>
        </a>
        <a
          href="https://forum.pinegrow.com/vue-designer"
          aria-label="facebook"
          external
          target="_blank"
        >
          <BaseIcon name="i-logos-discourse-icon"></BaseIcon>
        </a>
        <a
          href="https://www.youtube.com/@pinegrow/videos"
          aria-label="facebook"
          external
          target="_blank"
        >
          <BaseIcon name="i-logos-youtube-icon"></BaseIcon>
        </a>
      </div>
    </div>
  </div>
</template>
<style scoped></style>
