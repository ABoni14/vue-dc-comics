<template>
  <section>
    <div class="box">
      <img src="../assets/img/buy-comics-digital-comics.png" alt="">
      <h4>DIGITAL COMICS</h4>
    </div>
  </section>
</template>

<script>
export default {
  name: "SectionUnderMain",

  data(){
    return{
      boxs:[
        {
          url: "/digital-comics",
          img: "../assets/img/buy-comics-digital-comics.png",
          text: "digital comics"
        }
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
  }
</style>