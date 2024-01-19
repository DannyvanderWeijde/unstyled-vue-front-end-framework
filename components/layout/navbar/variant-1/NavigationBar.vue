<template>
  <nav>

  </nav>
</template>

<script setup lang="ts">
  defineProps({
    navbarItems: { type: Object, default() {return {}} },
    blockClass: { type: String, default: null }
  })
</script>