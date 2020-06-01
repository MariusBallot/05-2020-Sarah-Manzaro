<template>
  <div class="background"></div>
</template>

<script>
export default {
  name: "Background"
};
</script>

<!-- Add "scoped" attribute to limit CSS to this component only -->
<style scoped lang="stylus">
.background {
  width: 100vw;
  height: 100vh;
  background: black;
  position: absolute;
  top: 0;
  left: 0;
}
</style>
