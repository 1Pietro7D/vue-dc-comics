<template>
  <section class="pad-2">
    <div class="container-max">
      <a href="#">--> Content goes here &lt;--</a>
    </div>
  </section>
</template>

<script>
export default {
  name: "comp_sect_action",
};
</script>

<style lang="scss" scoped>
@import "@/css/variables.scss";
@import "@/css/generics.scss";
section {
  background-color: $sect_action_theme;
  font-family: "Noto Sans Myanmar", sans-serif;

  font-size: large;
  a {
    text-decoration: none;
    color: $white_theme;
  }
}
</style>
