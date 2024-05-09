<script lang="ts" setup>
const route = useRoute();
const enableCustomLayout = () => {
  route.meta.layout = 'custom';
}
definePageMeta({
  layout: false,
});
</script>
<template>
  <div>
    <button @click="enableCustomLayout">Update layout</button>
    <h1>About Page</h1>
  </div>
</template>