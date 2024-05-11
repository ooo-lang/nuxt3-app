<script setup>
const resetError = (error) => {
  error.value = null;
};
</script>
<template>
  <h1>Usersページ</h1>
  <NuxtErrorBoundary>
    <NuxtPage />
    <template #error="{ error }">
      <p>{{ error }}</p>
      <button @click="resetError(error)">Clear Error</button>
    </template>
  </NuxtErrorBoundary>
</template>