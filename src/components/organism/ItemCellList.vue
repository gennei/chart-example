<template>
  <div class="item-cells">
    <item-cell v-for="item in items" :key="item" />
  </div>
</template>

<script>
import ItemCell from "../../components/molecules/ItemCell.vue";
export default {
  components: {
    ItemCell
  },
  data: function() {
    return {
      items: [1, 2, 3, 4, 5, 6]
    };
  }
};
</script>
<style scoped>
.item-cells {
  width: 650px;
}
</style>