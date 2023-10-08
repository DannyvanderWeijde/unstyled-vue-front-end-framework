<template>
  <ul class="framework-navbar__list">
    <navbar-item-component
      v-for="(navbarItem, index) in navbarItems"
      :index="index"
      :item="navbarItem"
    ></navbar-item-component>
  </ul>
</template>

<script setup lang="ts">
  import NavbarItemComponent from './navbarItemComponent.vue'

  defineProps({
    navbarItems: {type: Object, default() {return {}}}
  })
</script>