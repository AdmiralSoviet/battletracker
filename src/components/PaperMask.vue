<template>
  <div class="paper-mask">
    <canvas></canvas>
  </div>
</template>

<script>
export default {
  name: "PaperMask",
};
</script>

<style scoped>
.paper-mask {
    display: none;
    position: absolute;
    top: 0;
    left: 0;
    height: 100%;
    width: 100%;
    z-index: 4;
}
.paper-mask canvas{
    width: 100%;
    height: 100%;
    z-index: 4;
}
</style>