<template>
  <img :src="url" :alt="alt" :width="width" />
</template>

<script>
export default {
  props: {
    url: String,
    alt: String,
    width: Number,
    height: Number
  }
};
</script>

<style scoped>
</style>