<template>
    <div class="product-card">
      <img :src="card.thumb" :alt="card.series">
      <h5 class="bianco uppercase">{{card.series}}</h5>
  </div>
</template>

<script>
export default {
    name : 'ProductsBox',
    props: ["card"]
}
</script>

<style lang="scss" scoped>
    @import '../style/commons.scss';
    @import '../style/commons-font.scss';

    .product-card {
      width: calc(100% / 5 - 50px);
      margin: 20px 0;

      img {
        width: 170px;
        height: 170px;
        object-fit: cover;
        object-position: top;
        margin-bottom: 10px;
        cursor: pointer;
      }
      h5 {
        cursor: pointer;
      }
    }

</style>