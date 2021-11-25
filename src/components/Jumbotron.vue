<template>
  <section class="jumbotron">
    <div class="container ab-relative">
      <div class="box-jumbotron">
        <h2>CURRENT BOX</h2>
      </div>
    </div> 
  </section>
</template>

<script>
export default {
  name: "Jumbotron",
}
</script>

<style lang="scss">

  @import "../assets/style/vars.scss";

  .jumbotron{
    height: 530px;
    min-height: 300px;
    background-image: url("../assets/img/jumbotron.jpg");
    background-repeat: no-repeat;
    background-size: cover;
    .ab-relative{
      height: 530px;
      position: relative;
      .box-jumbotron{
        background-color: $primary-color;
        height: 50px;
        position: absolute;
        left: 0;
        bottom: -25px;
        display: flex;
        justify-content: center;
        align-items: center;
        h2{
          padding: 10px 25px;
        }
      }
    }
    
  }
</style>