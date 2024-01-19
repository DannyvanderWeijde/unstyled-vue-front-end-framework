<template>
  <ul class="framework-navbar__list">
    <navigation-item
      v-for="(navbarItem, index) in navbarItems"
      :index="index"
      :item="navbarItem"
    ></navigation-item>
  </ul>
</template>

<script setup lang="ts">
  import NavigationItem from 'components/layout/navbar/variant-1/NavigationItem.vue'

  defineProps({
    navbarItems: {type: Object, default() {return {}}}
  })
</script>