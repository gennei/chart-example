<template>
  <div class="item-cell">
    <div class="image-container">
      <item-image
        src="https://m.media-amazon.com/images/I/51VSybdOnUL._SL160_.jpg"
        alt="容疑者Xの献身"
        width="40"
      />
    </div>
    <div class="item-attribute-container">
      <div class="row">
        <Title title="容疑者Xの献身" url="https://booklog.jp" />
      </div>
      <div class="row">
        <author name="東野圭吾" />
        <span class="separator">/</span>
        <genre />
        <span class="separator">/</span>
        <release-date />
        <span class="separator">/</span>
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
  padding: 10px;
  border-top: 1px solid;
  border-left: 1px solid;
  border-right: 1px solid;
  box-sizing: border-box;
  font-size: 12px;
}

.item-cell:last-child {
  border-bottom: 1px solid;
}

.item-attribute-container {
  display: flex;
  flex-direction: column;
  margin-left: 20px;
}

.row {
  margin-top: 10px;
}

.row:first-child {
  margin-top: 0px;
}

.separator {
  padding: 0 4px;
}
</style>