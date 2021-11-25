<template>
  <header>
    <div class="container header-contain">
      <img src="../assets/img/dc-logo.png" alt="">
      <ul class="header-nav">
        <li
        v-for="(link, index) in links" 
        :key="`ciclo-nav${index}`"
        :class="{active : (index === counter)}">
        <a
        class="nav-list"
        href="#">{{link.text}}</a></li>
      </ul>
    </div>
    
  </header>
</template>

<script>
export default {
  name: "Header",

  data(){
    return{
      links:[
        {
          url: "/characters",
          text: "characters",
          active: false,
        },
        {
          url: "/comic",
          text: "comic",
          active: false,
        },
        {
          url: "/movies",
          text: "movies",
          active: false,
        },
        {
          url: "/tv",
          text: "tv",
          active: false,
        },
        {
          url: "/games",
          text: "games",
          active: false,
        },
        {
          url: "/collectibles",
          text: "collectibles",
          active: false,
        },
        {
          url: "/videos",
          text: "videos",
          active: false,
        },
        {
          url: "/fans",
          text: "fans",
          active: false,
        },
        {
          url: "/news",
          text: "news",
          active: false,
        },
        {
          url: "/shop",
          text: "shop",
          active: false,
        },
      ],
      counter: 1,
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