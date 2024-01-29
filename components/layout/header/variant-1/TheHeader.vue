<template>
  <header :class="['framework-app-header', {'framework-app-header--sticky': sticky}]">
    <div v-if="$slots.left" :class="['framework-app-header__item framework-app-header__item--left', leftClass]">
      <slot name="left"></slot>
    </div>

    <div v-if="$slots.middle" :class="['framework-app-header__item framework-app-header__item--middle', middleClass]">
      <slot name="middle"></slot>
    </div>

    <div v-if="$slots.right" :class="['framework-app-header__item framework-app-header__item--right', rightClass]">
      <slot name="right"></slot>
    </div>
  </header>
</template>

<script setup lang="ts">
  defineProps({
    sticky: { type: Boolean, default: true },
    leftClass: {type: String, default: null},
    middleClass: {type: String, default: null},
    rightClass: {type: String, default: null}
  })
</script>