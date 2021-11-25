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
  .product-box{
    width: calc(100% / 6);
    margin-bottom: 30px;
    h3{
      color: white;
      text-transform: uppercase;
      font-size: 14px;
    }
    img{
      height: 250px;
      margin-bottom: 10px;
      object-fit: contain;
    }
  }
</style>