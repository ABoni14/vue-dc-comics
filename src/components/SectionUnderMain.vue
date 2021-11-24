<template>
  <section>
    <div class="container">
      <div class="box">
        <img src="../assets/img/buy-comics-digital-comics.png" alt="">
        <h4>DIGITAL COMICS</h4>
      </div>
      <div class="box">
        <img src="../assets/img/buy-comics-merchandise.png" alt="">
        <h4>DC MERCHANDISE</h4>
      </div>
      <div class="box">
        <img src="../assets/img/buy-comics-subscriptions.png" alt="">
        <h4>SUBSCRIPTIONS</h4>
      </div>
      <div class="box">
        <img src="../assets/img/buy-comics-shop-locator.png" alt="">
        <h4>COMIC SHOP LOCATOR</h4>
      </div>
      <div class="box">
        <img src="../assets/img/buy-dc-power-visa.svg" alt="">
        <h4>DC POWER VISA</h4>
      </div>
    </div>
    
  </section>
</template>

<script>
export default {
  name: "SectionUnderMain",

  data(){
    return{
      boxes:[
        {
          url: "/digital-comics",
          image: "../assets/img/buy-comics-digital-comics.png",
          text: "digital comics",
        },
        {
          url: "/dc-merchandise",
          image: "../assets/img/buy-comics-merchandise.png",
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
    justify-content: space-around;
    align-items: center;
    color: white;
    padding: 40px;
    .container{
      padding: 20px;
      .box{
        display: flex;
        align-items: center;
        img{
          width: 50px;
          margin-right: 5px;
        }
        h4{
          font-size: 15px;
        }
      }
    }
    
  }
</style>