<template>
  <section>
    <div
    v-for="(box, index) in boxes" 
    :key="`ciclo-box${index}`" 
    class="box">
      <img :src="`../assets/img/${box.image}`" :alt="box.url">
      <h4>{{box.text}}</h4>
    </div>
  </section>
</template>

<script>

import myImg from "../assets/img/buy-comics-digital-comics.png";

export default {
  name: "SectionUnderMain",

  data(){
    return{
      boxes:[
        {
          url: "/digital-comics",
          image: myImg,
          text: "digital comics",
        },
        {
          url: "/dc-merchandise",
          image: "buy-comics-merchandise.png",
          text: "dc merchandise",
        },
        {
          url: "/subscription",
          image: "../assets/img/buy-comics-subscriptions.png",
          text: "subscription",
        },
        {
          url: "/shop-locator",
          image: "../assets/img/buy-comics-shop-locator.png",
          text: "comic shop locator",
        },
        {
          url: "/dc-power-visa",
          image: "../assets/img/buy-dc-power-visa.svg",
          text: "dc power visa",
        },
      ]
    }
  }
}
</script>

<style lang="scss">
  @import "../assets/style/vars.scss";

  section{
    background-color: $primary-color;
    display: flex;
    justify-content: center;
    align-items: center;
    color: white;
    padding: 20px;
    .boxed{
      display: flex;
      align-items: center;
      img{
        width: 70px;
        margin-right: 5px;
      }
    }
  }
</style>