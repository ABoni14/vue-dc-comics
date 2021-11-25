<template>
  <section>
    <div class="container">
      <div 
      v-for="(box, index) in SectionMainData"
      :key="index"
      class="box">
        <img :src="box.image" :alt="box.alt">
        <h4>{{box.text}}</h4>
      </div>
    </div>
    
  </section>
</template>

<script>
import SectionMainData from "../assets/data/SectionMainData.js";

export default {
  
  data(){
    return{
      SectionMainData,
    }
  }
}
</script>

<style lang="scss">
  @import "../assets/style/vars.scss";

  section{
    background-color: $primary-color;
    display: flex;
    align-items: center;
    color: white;
    padding: 30px;
    .container{
      padding: 20px;
      display: flex;
    justify-content: space-between;

      .box{
        display: flex;
        align-items: center;
        img{
          width: 50px;
          margin-right: 5px;
        }
        h4{
          font-size: 15px;
          text-transform: uppercase;
        }
        .little-img{
          width: 38px;
        }
      }
    }
  }
</style>