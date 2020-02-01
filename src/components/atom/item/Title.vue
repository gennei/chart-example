<template>
  <a :href="url">
    <span>{{title}}</span>
  </a>
</template>

<script>
export default {
  props: {
    url: String,
    title: String
  }
};
</script>

<style scoped>
</style>