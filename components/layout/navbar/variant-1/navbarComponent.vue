<template>
  <header :class="['framework-app__header', {'framework-app__header--sticky': sticky}]">
    <nav class="framework-navbar">
      <div v-if="this.$slots.left" class="framework-navbar__left">
        <slot name="left"></slot>
      </div>

      <div v-if="this.$slots.middle" class="framework-navbar__middle">
        <slot name="middle"></slot>
      </div>

      <div v-if="this.$slots.right" class="framework-navbar__right">
        <slot name="right"></slot>
      </div>
    </nav>
  </header>
</template>

<script setup lang="ts">
  import NavbarItemComponent from './navbarItemComponent.vue'

  defineProps({
    navbarItems: { type: Object, default() {return {}} },
    sticky: { type: Boolean, default: true }
  })
</script>