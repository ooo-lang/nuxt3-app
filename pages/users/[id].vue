<script lang="ts" setup>
const router = useRoute();

console.log(router.params.id);
</script>

<template>
  <p>ユーザーID：{{  $route.params.id }}</p>
</template>