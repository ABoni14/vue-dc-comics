<template>
  <footer>
    <div class="container top-footer">
      <div class="list">
        <div class="col-list">
          <h3>DC COMICS</h3>
          <ul class="footer-list">
            <li><a href="">Characters</a></li>
            <li><a href="">Games</a></li>
            <li><a href="">Comics</a></li>
            <li><a href="">Movies</a></li>
            <li><a href="">Films</a></li>
            <li><a href="">News</a></li>
            <li><a href="">TV</a></li>
          </ul>

          <h3>SHOP</h3>
          <ul class="footer-list">
            <li><a href="">Shop DC</a></li>
            <li><a href="">Shop DC Collectibles</a></li>
          </ul>
        </div>
        <div class="col-list">
          <h3>DC</h3>
          <ul class="footer-list">
            <li><a href="">Characters</a></li>
            <li><a href="">Games</a></li>
            <li><a href="">Comics</a></li>
            <li><a href="">Movies</a></li>
            <li><a href="">Films</a></li>
            <li><a href="">News</a></li>
            <li><a href="">TV</a></li>
            <li><a href="">Films</a></li>
            <li><a href="">News</a></li>
            <li><a href="">TV</a></li>
          </ul>
        </div>
        <div class="col-list">
          <h3>SITES</h3>
          <ul class="footer-list">
            <li><a href="">DC</a></li>
            <li><a href="">MAD Magazine</a></li>
            <li><a href="">DC Kids</a></li>
            <li><a href="">DC Universe</a></li>
            <li><a href="">DC Power Visa</a></li>
          </ul>
        </div>
      </div>
      <div class="footer-img">
        <img src="../assets/img/dc-logo-bg.png" alt="">
      </div>
    </div>
    <div class="bottom-footer">
      <div class="container">
        <button>SIGN-UP NOW!</button>
        <div class="footer-contain-right">
          <h3>FOLLOW US</h3>
          <img src="../assets/img/footer-facebook.png" alt="">
          <img src="../assets/img/footer-twitter.png" alt="">
          <img src="../assets/img/footer-youtube.png" alt="">
          <img src="../assets/img/footer-pinterest.png" alt="">
          <img src="../assets/img/footer-periscope.png" alt="">
        </div>
      </div>
    </div>
  </footer>
</template>

<script>
export default {
  name: "Footer"
}
</script>

<style lang="scss">
  @import "../assets/style/vars.scss";

  footer{
    background-image: url("../assets/img/footer-bg.jpg");
    .top-footer{
      height: 400px;
      color: white;
      display: flex;
      justify-content: space-between;
      align-items: center;
      overflow: hidden;
      .list{
        display: flex;
        .col-list{
          margin-right: 30px;
          .footer-list{
            display: flex;
            flex-direction: column;
            li a{
              margin-left: -10px;
              color: rgb(189, 189, 189);
              text-transform: unset;
            }
          }
        }
      }
      h3{
        font-size: 25px;
        margin: 10px 0;
      }
    } 
  }
  .footer-img{
    img{
      width: 100%;
    }
  }
  .bottom-footer{
    background-color: #303030;
    .container{
      display: flex;
      justify-content: space-between;
      align-items: center;
      button{
        background-color: #303030;
        border: 2px solid $primary-color;
        color: white;
        padding: 10px;
      }
      .footer-contain-right{
        display: flex;
        justify-content: space-between;
        align-items: center;
        h3{
          color: $primary-color;
          margin-right: 10px;
        }
        img{
          width: 35px;
          margin-left: 10px;
        }
      }
    }
  }
</style>