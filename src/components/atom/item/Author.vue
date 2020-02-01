<template>
  <a v-if="url" :href="url">
    <span class="author-name">{{name}}</span>
  </a>
  <span v-else class="author-name">{{name}}</span>
</template>

<script>
export default {
  props: {
    url: String,
    name: String
  }
};
</script>

<style scoped>
</style>