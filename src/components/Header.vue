<template>
  <header>
    <div class="container">
      <img src="../assets/img/dc-logo.png" alt="">
      <ul>
        <li
        v-for="(link, index) in links" :key="index"
        ><a href="#">{{link.text}}</a></li>
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
      ]
    }
  }

}
</script>

<style lang="scss">
  @import "../assets/style/vars.scss";

  .container{
    height: 100px;
    // width: 1100px;
    // margin: 0 auto;
    display: flex;
    justify-content: space-between;
    align-items: center;
    ul li{
      list-style: none;
      display: inline-block;
      a{
        text-decoration: none;
        color: black;
        padding: 10px;
        font-weight: 500;
        text-transform: uppercase;
        &:hover{
          color: $primary-color;
          border-bottom: 2px solid $primary-color;
        }
      }
    }
    img{
      width: 70px;
    }
  }
</style>