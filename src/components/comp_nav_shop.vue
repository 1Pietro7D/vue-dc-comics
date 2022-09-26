<template>
  <div class="card">
    <div class="card_img">
      <img :src="url" :alt="text" />
    </div>
    <p>{{ text }}</p>
  </div>
</template>

<script>
export default {
  name: "shop_comp",
  props: { url: String, text: String },
};
</script>

<style lang="scss" scoped>
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
</style>
