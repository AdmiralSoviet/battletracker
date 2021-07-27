<template>
  <div class="init-block">
    <input type="text" class="init-name" v-bind:value="nme" />
    <input type="number" class="init-roll" v-bind:value="roll" />
  </div>
</template>

<script>
export default {
  name: "Tile",
  props: {
    nme: String,
    roll: String,
  },
};
</script>

<style scoped>
.init-block {
  border-radius: 2px;
  height: 43px;
  font-family: "Source Serif Pro", sans-serif;
  margin-top: 5px;
  margin-bottom: 5px;
  margin-top: 5px;
  margin-bottom: 5px;
  padding: 5px;
  transition: 0.15s;
}

.init-block:hover{
    background: rgba(0, 0, 0, 0.2);
}
.init-block input {
  border: none;
  color: inherit;
}
.init-name {
  padding: 10px;
  width: calc(100% - 75px);
  float: left;
  background: linear-gradient(180deg, #cf9e52 0, #cf9e52 98%);
  background-size: 100% 2px;
  background-repeat: no-repeat;
  background-position: left 100%;
  font-size: 20px;
  font-family: "IM Fell Great Primer SC",serif;
}
.init-name:focus-visible, .init-roll:focus-visible{
    text-decoration: none;
    border: none;
    outline: none;
}
.init-roll {
  padding-left: 10px;
  padding-top: 9px;
  padding-bottom: 10px;
  width: 35px;
  float: right;
  font-size: 20px;
  background: #cf9e52;
  font-family: inherit;
}
</style>