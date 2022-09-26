<template>
  <main>
    <jumbo_tron />
    <comp_sect_action />
    <comp_sect_shop />
  </main>
</template>

<script>
import jumbo_tron from "@/components/jumbo_tron.vue";
import comp_sect_action from "@/components/comp_sect_action.vue";
import comp_sect_shop from "@/components/comp_sect_shop.vue";

export default {
  name: "comp_main",

  components: {
    jumbo_tron,
    comp_sect_action,
    comp_sect_shop,
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
