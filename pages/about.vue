<script lang="ts" setup>
const route = useRoute();
const title = ref('About ページ');
const description = ref('Aboutページ');
const enableCustomLayout = () => {
  route.meta.layout = 'custom';
}

useHead({
  title,
  meta: [
    {
      name: 'description',
      content: description,
    }
  ]
})


</script>
<template>
  <div>
    <button @click="enableCustomLayout">Update layout</button>
    <h1>About Page</h1>
  </div>
</template>