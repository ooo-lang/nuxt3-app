<script lang="ts" setup>
useHead({
  titleTemplate: (title?: string) => {
    return title ? `${title} - Nuxt 3 basic` : `Nuxt 3 basic`;
  },
});
</script>

<template>
  <div>
    <Navbar />
    <slot />
  </div>
</template>

<style>
.page-enter-active,
.page-leave-active {
  transition: all 0.4;
}
.page-enter-from,
.page-leave-to {
  opacity: 0;
  filter: blur(5rem);
}
</style>
