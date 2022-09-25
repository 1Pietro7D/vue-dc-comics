<template>
  <div id="app">
    <comp_header />
    <comp_main />
  </div>
</template>

<script>
import comp_header from "./components/comp_header.vue";
import comp_main from "@/components/comp_main.vue";

export default {
  name: "App",
  data() {},
  components: {
    comp_header,
    comp_main,
  },
};
</script>

<style lang="scss">
@import "@/css/generics.scss";
/* global reset */
* {
  margin: 0;
  padding: 0;
  box-sizing: border-box;
}
.container-max {
  max-width: 1200px;
  margin: auto;
}
</style>

<!--
@import "@/css/generics.scss";
@import "@/css/variables.scss";
@import "@/css/position.scss"; 
@import "@/css/display.scss";
@import "@/css/flex.scss";
@import "@/css/grid.scss"; 
-->
