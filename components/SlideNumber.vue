<template>
  <span v-if="$frontmatter.footer !== false" class="image-slide-number">{{ $slidev.nav.currentPage }}</span>
</template>
