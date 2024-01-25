<template>
  <header :class="['framework-app__header', {'framework-app__header--sticky': sticky}, blockClass]">
    <div v-if="$slots.left" class="framework-app__header-item framework-app__header-item--left">
      <slot name="left"></slot>
    </div>

    <div v-if="$slots.middle" class="framework-app__header-item framework-app__header-item--middle">
      <slot name="middle"></slot>
    </div>

    <div v-if="$slots.right" class="framework-app__header-item framework-app__header-item--right">
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