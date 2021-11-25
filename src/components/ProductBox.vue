<template>
  <div class="product-box">
    <img :src="product.thumb" :alt="product.type">
    <h3>{{product.series}}</h3>
  </div>
</template>

<script>
export default {
  name: "ProductBox",
  props:{
    product: Object,
  }
}
</script>

<style lang="scss">

  @import "../assets/style/vars.scss";

  .product-box{
    width: calc(100% / 6);
    margin-bottom: 20px;
    padding: 13px;
    h3{
      color: $white-text;
      text-transform: uppercase;
      font-size: 14px;
    }
    img{
      width: 100%;
      height: 160px;
      margin-bottom: 10px;
      object-fit: cover;
      object-position: top;
    }
  }
</style>