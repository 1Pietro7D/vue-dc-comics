<template>
  <div>
    <div v-if="clicked">
      vorrei collegarlo al click su comp_sect_action.vue ... ma niente ...
      potrei provare alterando le classi.. ma...o con un props???
    </div>
    <div v-else id="jumbo_tron">
      <img src="@/assets/img/jumbotron.jpg" alt="" />
    </div>
  </div>
</template>

<script>
export default {
  name: "jumbo_tron",
};
</script>

<style lang="scss" scoped>
#jumbo_tron {
  width: 100%;
  height: calc(100vw / 4);
  img {
    width: 100%;
    height: 100%;
    object-fit: cover;
    object-position: 0 0;
  }
}
</style>
