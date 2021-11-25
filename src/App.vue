<template>
  <div>
    <Header />
    <Jumbotron />
    <Main />
    <SectionUnderMain />
    <Footer />
  </div>
</template>

<script>
import Header from "./components/Header.vue";
import Jumbotron from "./components/Jumbotron.vue";
import Main from "./components/Main.vue";
import SectionUnderMain from "./components/SectionUnderMain.vue";
import Footer from "./components/Footer.vue";

export default {
  name: 'App',
  components: {
    Header,
    Jumbotron,
    Main,
    SectionUnderMain,
    Footer
  }
}
</script>

<style lang="scss">
@import "./assets/style/vars.scss";
@import "./assets/style/general.scss";
@import "./assets/style/utilities.scss";
</style>
