<template>
  <div id="app">
    <Chart />
    <item-cell-list />
  </div>
</template>

<script>
import Chart from "./components/Chart.vue";
import ItemCellList from "./components/organism/ItemCellList.vue";

export default {
  name: "app",
  components: {
    Chart,
    ItemCellList
  }
};
</script>

<style>
#app {
  font-family: "Avenir", Helvetica, Arial, sans-serif;
  -webkit-font-smoothing: antialiased;
  -moz-osx-font-smoothing: grayscale;
  text-align: center;
  color: #2c3e50;
  margin-top: 60px;
}
</style>
