<template>
  <section class="framework-app-menu">
    <div class="framework-app-menu__header">
      <slot name="header"></slot>
    </div>
    <div class="framework-app-menu__body">
      <slot name="body"></slot>
    </div>
  </section>
</template>

<script>
  export default {
    name: 'TheMenu'
  }
</script>