<template>
  <div id="side-content">
    <img src="./assets/logo.png" alt="Logo"/>
    <PaperMask />
    <Initiative />
  </div>
  <div id="home-main">
    <Board />
  </div>
</template>

<script>
import Initiative from "./components/Initiative.vue";
import Board from "./components/Board.vue";
import PaperMask from "./components/PaperMask.vue";
import "./assets/style.css";

export default {
  name: "App",
  components: {
    Initiative,
    Board,
    PaperMask
  },
};
</script>

<style scoped>
#side-content {
  position: absolute;
  background: #e0dace;
  height: 100%;
  top: 0;
  left: 0;
  width: 24rem;
  z-index: 3;
  box-shadow: 0 0 1.7rem 2px rgb(49 50 50 / 25%);
}
#side-content img{
  width: 100%;
}
#home-main {
  position: absolute;
  width: calc(100% - 24rem);
  height: 100%;
  background: rgb(160 153 142 / 69%);
  left: 24rem;
  z-index: 1;
}
</style>