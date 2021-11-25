<template>
  <header>
    <div class="container header-contain">
      <img src="../assets/img/dc-logo.png" alt="">
      <ul class="header-nav">
        <li
        v-for="(link, index) in Links" 
        :key="`ciclo-nav${index}`"
        :class="{active : (index === counter)}"
        @click="counter = index">
        <a
        class="nav-list"
        href="#">{{link.text}}</a></li>
      </ul>
    </div>
    
  </header>
</template>

<script>
import Links from "../assets/data/LinksHeaderData";

export default {
  name: "Header",

  data(){
    return{
      Links,
      counter: 0,
    }
  }
}
</script>

<style lang="scss">
  @import "../assets/style/vars.scss";

  header{
    height: 100px;
    .container{
      display: flex;
      justify-content: space-between;
      align-items: center;
      .header-nav li{
        list-style: none;
        display: inline-block;
        cursor: pointer;
        &:hover a{
          color: $primary-color;
        }
        &:hover,
        &.active{
          border-bottom: 4px solid $primary-color;
          margin-bottom: -4px;
          }
        &.active a{
          color: $primary-color;
        }
        a{
          text-decoration: none;
          color: black;
          padding: 10px;
          text-transform: uppercase;
          line-height: 96px;
          font-weight: 700;
        }
      }
      img{
        width: 70px;
        cursor: pointer;
      }
      .nav-list{
        line-height: 100px;
      }
    }
  }
</style>