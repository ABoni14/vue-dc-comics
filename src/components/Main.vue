<template>
  <main>
    <div class="container ab-boxes">
      <ProductBox
      v-for="(product, index) in MainData"  
      :key="index" 
      :product="product" />
    </div>

    <div class="container ab-button-main">
      <button><a href="#">LOAD MORE</a></button>
    </div>
  </main>
</template>

<script>
import ProductBox from "./ProductBox.vue";
import MainData from "../assets/data/MainData";

export default {
  name: "Main",
  components:{
    ProductBox
  },
  data(){
    return{
      MainData,
    }
  }
}
</script>

<style lang="scss">

  @import "../assets/style/vars.scss";

  main{
    background-color: #1c1c1c;
    padding: 60px 0 20px 0;
    .ab-boxes{
      display: flex;
      flex-wrap: wrap;
    }
    .ab-button-main{
      text-align: center;
      button{
        background-color: $primary-color;
        padding: 10px 60px;
        border: none;
        margin-top: 30px;
        a{
          color: white;
          text-decoration: none;
          font-weight: 700;
        }
      }
    }
    
  }
  
</style>