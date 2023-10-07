<template>
  <router-link :to="{name: index}">
    {{ item }}
  </router-link>
</template>

<script setup lang="ts">
  defineProps({
    index: {type: String, default: null },
    item: {type: String, default: null },
  })
</script>