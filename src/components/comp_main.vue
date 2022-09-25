<template>
  <main>
    <jumbo_tron />
    <comp_sect_action />
  </main>
</template>

<script>
import comp_sect_action from "@/components/comp_sect_action.vue";
import jumbo_tron from "@/components/jumbo_tron.vue";

export default {
  name: "comp_main",

  components: {
    comp_sect_action,
    jumbo_tron,
  },
};
</script>

<style lang="scss" scoped></style>

<!--
  @import "@/css/generics.scss";
  @import "@/css/variables.scss";
  @import "@/css/position.scss"; 
  @import "@/css/display.scss";
  @import "@/css/flex.scss";
  @import "@/css/grid.scss"; 
  -->
