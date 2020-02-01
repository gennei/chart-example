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
      items: [1, 2]
    };
  }
};
</script>