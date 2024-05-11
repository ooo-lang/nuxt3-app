<script setup>
const counter = ref(0);
const inc = () => {
  throw createError('Error発生')
  counter.value++;
}
</script>
<template>
  <h1>User List</h1>
  <h2>Counter</h2>
  <p>Count: {{ counter }}</p>
  <div><button @click="inc">+</button></div>
</template>