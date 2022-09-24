<template>
  <div id="app">
    <comp_header />
  </div>
</template>

<script>
import comp_header from "./components/comp_header.vue";

export default {
  name: "App",
  components: {
    comp_header,
  },
};
</script>

<style lang="scss">
#app {
  font-family: Avenir, Helvetica, Arial, sans-serif;
  -webkit-font-smoothing: antialiased;
  -moz-osx-font-smoothing: grayscale;
}
</style>
