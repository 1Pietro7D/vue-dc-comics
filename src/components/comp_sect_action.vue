<template>
  <section class="pad-y-2 relative">
    <div class="container-max">
      <div v-if="clicked" id="current_series">current series</div>
      <a v-if="!clicked" @click="click" href="#"
        >--> Content goes here &lt;--</a
      >
      <div id="album" class="d-grid pad-2" v-else>
        <comp_cards
          v-for="(card, index) in cards"
          :key="index"
          :url="cards[index].thumb"
          :price="cards[index].price"
          :title="cards[index].series"
          :type="cards[index].type"
        />
      </div>
      <div class="btn_brand" v-if="clicked">LOAD MORE</div>
    </div>
  </section>
</template>

<script>
import { cards } from "@/data/dc-comics.js";
import comp_cards from "@/components/comp_cards.vue";
export default {
  name: "comp_sect_action",

  data() {
    return {
      cards,
      clicked: false,
    };
  },
  components: { comp_cards },
  methods: {
    click() {
      return (this.clicked = true);
    },
  },
};
</script>

<style lang="scss" scoped>
@import "@/css/variables.scss";
@import "@/css/generics.scss";
@import "@/css/grid.scss";
@import "@/css/position.scss";

section {
  background-color: $sect_action_theme;
  font-family: "Noto Sans Myanmar", sans-serif;
  color: $white_theme;
  font-size: large;
  a {
    text-decoration: none;
    color: $white_theme;
  }
  .d-grid {
    @include grid-col-1;

    @media screen and (min-width: 480px) {
      @include grid-col-2;
    }
    @media screen and (min-width: 780px) {
      @include grid-col-4;
    }
    @media screen and (min-width: 1200px) {
      @include grid-col-6;
    }
    @media screen and (max-width: 1200px) {
      padding: 2rem 3rem;
    }
  }

  #current_series {
    background-color: $blue_primary;
    padding: 1rem;
    color: $white_theme;
    text-transform: uppercase;
    position: absolute;
    top: 0px;
    transform: translateY(-50%);
  }
  .btn_brand {
    background-color: $brand_theme;
    display: inline-block;
    padding: 0.5rem;
    /* STRANAMENTE NON RIESCO A CENTRARLO CON IL MARGIN, FORSE FLEX?? */
    @include relativeX-center;
  }
}
</style>
