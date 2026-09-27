<script setup lang="ts">
defineProps<{ hideNumber?: boolean }>()
</script>

<template>
  <footer v-if="$frontmatter.footer !== false" class="deck-footer">
    <span>{{ $frontmatter.footer || $slidev.configs.title }}</span>
    <span v-if="!hideNumber">{{ $slidev.nav.currentPage }}</span>
  </footer>
</template>
