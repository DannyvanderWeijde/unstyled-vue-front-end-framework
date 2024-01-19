<template>
  <header :class="['framework-app__header', {'framework-app__header--sticky': sticky}, blockClass]">
    <div v-if="$slots.left" class="framework-app__header-item">
      <slot name="left"></slot>
    </div>

    <div v-if="$slots.middle" class="framework-app__header-item">
      <slot name="middle"></slot>
    </div>

    <div v-if="$slots.right" class="framework-app__header-item">
      <slot name="right"></slot>
    </div>
  </header>
</template>

<script setup lang="ts">
  defineProps({
    sticky: { type: Boolean, default: true },
    blockClass: { type: String, default: null }
  })
</script>