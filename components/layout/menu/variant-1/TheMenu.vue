<template>
  <section class="framework-app-menu">
    <div v-if="$slots.header" class="framework-app-menu__header">
      <slot name="header"></slot>
    </div>
    <div v-if="$slots.body" class="framework-app-menu__body">
      <slot name="body"></slot>
    </div>
  </section>
</template>

<script>
  export default {
    name: 'TheMenu'
  }
</script>