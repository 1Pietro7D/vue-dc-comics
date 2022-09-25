<template>
  <div>
    <div class="miao">ciao</div>
  </div>
</template>

<script>
export default {
  name: "comp_header",
  props: {
    // msg: String
  },
};
</script>

<!-- Add "scoped" attribute to limit CSS to this component only -->
<style scoped lang="scss">
@import "@/css/variables";
@import "@/css/generics.scss";
@import "@/css/position.scss";
@import "@/css/display.scss";
@import "@/css/flex.scss";
@import "@/css/grid.scss";
.miao {
  @include absolute-center;
  color: red;
  background-color: $blue_brand;
}
</style>
