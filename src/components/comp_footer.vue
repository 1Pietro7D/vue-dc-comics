<template>
  <footer>
    <nav class="d-flex">
      <div class="container-max"></div>
    </nav>
    <section class="pad-2">
      <div class="container-max d-flex justify-between">
        <div>
          <a href="#">SING UP</a>
        </div>
        <div id="icon-container"></div>
      </div>
    </section>
  </footer>
</template>

<script>
export default {
  name: "comp_footer",
};
</script>

<style lang="scss" scoped>
@import "@/css/generics.scss";
@import "@/css/variables.scss";
@import "@/css/position.scss";
@import "@/css/display.scss";
@import "@/css/flex.scss";
@import "@/css/grid.scss";
footer {
  color: $white_theme;
  a {
    text-decoration: none;
    color: $white_theme;
  }
  nav {
    height: 600px;
    background-image: url(../assets/img/footer-bg.jpg);
    background-size: cover;
  }
  section {
    background-color: $footer_theme;
  }
}
</style>
