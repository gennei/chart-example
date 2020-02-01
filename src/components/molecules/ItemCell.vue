<template>
  <div class="item-cell">
    <div class="image-container">
      <item-image src="https://m.media-amazon.com/images/I/51VSybdOnUL._SL160_.jpg" alt="容疑者Xの献身" />
    </div>
    <div class="item-attribute-container">
      <div class="row">
        <Title title="容疑者Xの献身" url="https://booklog.jp" />
      </div>
      <div class="row">
        <author name="東野圭吾" />
        <span>/</span>
        <genre />
        <span>/</span>
        <release-date />
        <span>/</span>
        <store />
      </div>
    </div>
  </div>
</template>

<script>
import ItemImage from "../../components/atom/item/ItemImage.vue";
import Title from "../../components/atom/item/Title.vue";
import Author from "../../components/atom/item/Author.vue";
import Genre from "../../components/atom/item/Genre.vue";
import ReleaseDate from "../../components/atom/item/ReleaseDate.vue";
import Store from "../../components/atom/item/Store.vue";

export default {
  components: {
    ItemImage,
    Title,
    Author,
    Genre,
    ReleaseDate,
    Store
  }
};
</script>

<style scoped>
.item-cell {
  display: flex;
  text-align: left;
}
.item-attribute-container {
  display: flex;
  flex-direction: column;
}
</style>