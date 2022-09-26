<template>
  <header>
    <div
      class="container-max d-flex justify-between container-max align-center"
    >
      <div class="logo_DC">
        <img src="@/assets/img/dc-logo.png" alt="" />
      </div>
      <nav>
        <ul class="d-flex gap-1 h-100">
          <comp_links
            v-for="(item, index) in links"
            :key="index"
            :text="links[index].label"
            :url="links[index].url"
          />
        </ul>
      </nav>
    </div>
  </header>
</template>

<script>
import comp_links from "./comp_links.vue";
import { links } from "@/data/header_link.js";

export default {
  name: "comp_header",
  data() {
    return {
      links,
    };
  },
  components: {
    comp_links,
  },
};
</script>

<!-- Add "scoped" attribute to limit CSS to this component only -->
<style scoped lang="scss">
@import "@/css/variables.scss";
@import "@/css/flex.scss";
@import "@/css/generics.scss";
header {
  background-color: $header_theme;
  font-family: "Fredoka One";
}
nav {
  @media screen and (max-width: 850px) {
    display: none;
  }
}

.logo_DC {
  display: inline-block;
  width: 50px;
  height: 50px;
  img {
    width: 100%;
    height: 100%;
  }
}
</style>
