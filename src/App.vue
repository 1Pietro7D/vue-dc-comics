<template>
  <div id="app">
    <comp_header />
    <comp_sect_action />
  </div>
</template>

<script>
import comp_header from "./components/comp_header.vue";
import comp_sect_action from "@/components/comp_sect_action.vue";
import links from "@/data/header_link";

export default {
  name: "App",
  data() {
    return {
      links,
    };
  },
  components: {
    comp_header,
    comp_sect_action,
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
