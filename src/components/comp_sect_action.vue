<template>
  <section class="pad-y-2 relative">
    <div class="container-max">
      <div v-if="clicked" id="current_series">current series</div>
      <a v-if="!clicked" @click="click" href="#"
        >--> Content goes here &lt;--</a
      >
      <div id="album" class="grid-col-6 pad-y-2" v-else>
        <div class="cards" v-for="(x, index) in 12" :key="index"></div>
      </div>
    </div>
  </section>
</template>

<script>
export default {
  name: "comp_sect_action",
  data() {
    return {
      clicked: false,
    };
  },
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
  .grid-col-6 {
    @include grid-col-6;
    gap: 1rem;
  }
  .cards {
    height: 50px;
    background-color: red;
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
}
</style>
