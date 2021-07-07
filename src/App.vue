<template>
  <div id="app">
    <Header/>
    <Jumbotron/>
    <!-- <Main/> -->
    <FooterUp/>
    <FooterCentre/>
    <FooterSocial/>
    <!-- <img alt="Vue logo" src="./assets/logo.png">
    <HelloWorld msg="Welcome to Your Vue.js App"/> -->
  </div>
</template>

<script>
// import HelloWorld from './components/HelloWorld.vue'
import Header from './components/Header.vue';
import FooterUp from './components/FooterUp.vue';
import FooterCentre from './components/FooterCentre.vue';
import FooterSocial from './components/FooterSocial.vue';
import Jumbotron from './components/Jumbotron.vue';




export default {
  name: 'App',
  components: {
    // HelloWorld
    Header,
    FooterUp,
    FooterCentre,
    FooterSocial,
    Jumbotron
  }
}
</script>

<style lang="scss">
// #app {
  // font-family: Avenir, Helvetica, Arial, sans-serif;
  // -webkit-font-smoothing: antialiased;
  // -moz-osx-font-smoothing: grayscale;
  // text-align: center;
  // color: #2c3e50;
  // margin-top: 60px;
// }
</style>
