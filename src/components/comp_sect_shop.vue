<template>
  <section class="pad-y-2">
    <div class="container-max">
      <nav class="d-grid">
        <shop_comp
          v-for="(card, index) in shop"
          :key="index"
          :url="shop[index].url"
          :text="shop[index].description"
        />
      </nav>
    </div>
  </section>
</template>

<script>
import shop_comp from "./comp_nav_shop.vue";
import { shop } from "@/data/shop";
export default {
  name: "comp_sect_shop",
  components: { shop_comp },
  data() {
    return {
      shop,
    };
  },
};
</script>

<style lang="scss" scoped>
@import "@/css/flex.scss";
@import "@/css/generics.scss";
@import "@/css/variables.scss";
@import "@/css/grid.scss";
section {
  background-color: $blue_primary;
  color: $white_theme;
  .d-grid {
    @include grid-col-1;
    @media screen and (min-width: 480px) {
      @include grid-col-2;
    }
    @media screen and (min-width: 780px) {
      @include grid-auto-col-5;
      gap: 2rem;
    }
    @media screen and (max-width: 780px) {
      padding: 2rem 3rem;
    }
  }
}
</style>
