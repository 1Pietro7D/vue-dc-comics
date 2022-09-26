<template>
  <section class="pad-y-2">
    <div class="container-max">
      <nav class="d-grid">
        <div class="card">
          <div class="card_img">
            <img src="@/assets/img/buy-comics-digital-comics.png" alt="" />
          </div>
          <p>DIGITAL COMICS</p>
        </div>
        <div class="card">
          <div class="card_img">
            <img src="@/assets/img/buy-comics-merchandise.png" alt="" />
          </div>
          <p>DC merchandise</p>
        </div>
        <div class="card">
          <div class="card_img">
            <img src="@/assets/img/buy-comics-subscriptions.png" alt="" />
          </div>
          <p>subscription</p>
        </div>
        <div class="card">
          <div class="card_img">
            <img src="@/assets/img/buy-comics-shop-locator.png" alt="" />
          </div>
          <p>comic shop locator</p>
        </div>
        <div class="card">
          <div class="card_img">
            <img src="@/assets/img/buy-dc-power-visa.svg" alt="" />
          </div>
          <p>DC power visa</p>
        </div>
      </nav>
    </div>
  </section>
</template>

<script>
export default { name: "comp_sect_shop" };
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
  .card {
    display: flex;
    gap: 1rem;
    align-items: center;
    margin: auto;
    text-transform: uppercase;
    @media screen and (max-width: 780px) {
      flex-direction: column;
    }
    .card_img {
      $size: 70px;
      width: $size;
      height: $size;
      img {
        width: 100%;
        height: 100%;
        object-fit: scale-down;
      }
    }
  }
}
</style>
