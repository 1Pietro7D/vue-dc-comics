<template>
  <footer>
    <div id="nav-container">
      <div class="d-flex justify-between container-max pad-0">
        <nav class="d-flex pad-2 gap-2">
          <div>
            <ul>
              <h2>dc comics</h2>
              <li></li>
            </ul>
            <ul>
              <h2>shop</h2>
              <li></li>
            </ul>
          </div>
          <ul>
            <h2>dc</h2>
            <li></li>
          </ul>
          <ul>
            <h2>sites</h2>
            <li></li>
          </ul>
        </nav>
        <div class="jumbo-img">
          <img src="../assets/img/dc-logo-bg.png" alt="" />
        </div>
      </div>
    </div>
    <section>
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
  #nav-container {
    $height: 450px;
    height: $height;
    background-image: url(../assets/img/footer-bg.jpg);
    background-size: cover;
    .jumbo-img {
      width: 650px;
      height: $height;
      img {
        width: 100%;
        height: 100%;
        object-fit: cover;
        @media screen and (max-width: 1200px) {
          display: none;
        }
      }
    }
  }
  section {
    background-color: $footer_theme;
  }
}
</style>
