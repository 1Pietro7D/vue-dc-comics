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
/* global reset */
* {
  margin: 0;
  padding: 0;
  box-sizing: border-box;
}
</style>

<!--
@import "./css/generics.scss";
@import "./css/variables.scss";
@import "@/css/position.scss"; 
@import "@/css/display.scss";
@import "@/css/flex.scss";
@import "@/css/grid.scss"; 
-->
