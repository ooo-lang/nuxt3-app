<script lang="ts" setup>
const { count, inc, dec } = useCounter(100);
const { $hello } = useNuxtApp();
</script>
<template>
  <div>
    <h1>Main Page</h1>
    <h2>{{ $hello('World') }}</h2>
    <div>
      Count: {{ count }}
    </div>
    <div>
      <button @click="() => inc()">increment</button>
      <button @click="() => dec()">decrement</button>
    </div>
  </div>
</template>