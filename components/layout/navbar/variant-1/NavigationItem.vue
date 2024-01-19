<template>
  <router-link :to="{name: index}" class="framework-navbar__list-item">
    {{ item }}
  </router-link>
</template>

<script setup lang="ts">
  defineProps({
    index: {type: String, default: null },
    item: {type: String, default: null },
  })
</script>