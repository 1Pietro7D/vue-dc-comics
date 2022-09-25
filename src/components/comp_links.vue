<template>
  <li>
    <a href="url">{{ text }}</a>
  </li>
</template>

<script>
export default {
  name: "comp_links",
  props: {
    text: String,
    url: String,
  },
};
</script>

<!-- Add "scoped" attribute to limit CSS to this component only -->
<style scoped lang="scss">
@import "@/css/variables.scss";
@import "@/css/generics.scss";
li {
  display: flex;
  align-items: center;
}
a {
  text-decoration: none;
  text-transform: uppercase;
  color: $dark_grey;
}
</style>
