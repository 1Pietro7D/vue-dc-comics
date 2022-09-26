<template>
  <div class="card pad-1">
    <div class="card_img">
      <img :src="url" :alt="type" />
    </div>
    <span>{{ title }}</span>
  </div>
</template>

<script>
export default {
  name: "comp_links",
  props: {
    url: String,
    price: String,
    title: String,
    type: String,
  },
};
</script>

<!-- Add "scoped" attribute to limit CSS to this component only -->
<style scoped lang="scss">
@import "@/css/variables.scss";
@import "@/css/generics.scss";
.card {
  .card_img {
    height: 100vw;
    @media screen and (min-width: 480px) {
      height: 50vw;
    }
    @media screen and (min-width: 780px) {
      height: 25vw;
    }
    @media screen and (min-width: 1200px) {
      height: 220px;
    }
    img {
      width: 100%;
      height: 100%;
      object-fit: cover;
      object-position: 0 0;
    }
  }
}
</style>
