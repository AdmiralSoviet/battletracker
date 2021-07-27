<template>
  <div class="initiative">
    <h2>Order of Battle</h2>
    <p>The initiative ladder, top goes first.</p>
    <Tile nme="Falius The Wise" roll="19" />
    <Tile nme="Jamal Saxon" roll="13" />
    <Tile nme="Enemies" roll="2" />
  </div>
</template>

<script>
import Tile from "./Tile.vue";
export default {
  name: "Initiative",
  components: {
    Tile
  },
};
</script>

<style scoped>
.initiative {
  padding: 5px;
  padding-left: 20px;
  padding-right: 20px;
  z-index: 5;
}
h1 {
  margin: 0px;
}
h2 {
  text-align: center;
  font-size: 28px;
  margin-top: 15px;
  margin-bottom: 9.6px;
}
p {
    font-size: 14px;
    text-align: center;
    margin: 0px;
}
</style>