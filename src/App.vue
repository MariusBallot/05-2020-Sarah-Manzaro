<template>
  <div id="app">
    <ComingSoon />
  </div>
</template>

<script>
import ComingSoon from "./components/ComingSoon.vue";

export default {
  name: "App",
  components: {
    ComingSoon
  }
};
</script>

<style lang="stylus">
@import url('https://fonts.googleapis.com/css2?family=Playfair+Display:wght@500&family=Raleway:wght@400;700&display=swap');

body {
  width: 100vw;
  height: 100vh;
  overflow: hidden;
}

* {
  margin: 0;
  padding: 0;
  box-sizing: border-box;
  font-family: 'Raleway', sans-serif;
}

h1, h2, h3 {
  font-family: 'Playfair Display';
}

a {
  color: inherit;
  text-decoration: none;
}
</style>
