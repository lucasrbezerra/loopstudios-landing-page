<template>
  <div id="app">
    <banner />
    <about />
    <our-creations />
    <Footer />
  </div>
</template>

<script>
import Banner from "../layouts/Banner";
import About from "../layouts/About";
import OurCreations from "../layouts/OurCreations";
import Footer from "../layouts/Footer";
export default {
  components: {
    Banner,
    About,
    OurCreations,
    Footer,
  },
};
</script>

<style lang="scss">
html,
body,
#app {
  margin: 0;
  padding: 0;
  box-sizing: border-box;
  width: 100%;
  height: 100%;
}
</style>
