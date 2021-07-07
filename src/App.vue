<template>
  <div id="app">
    <Header/>
    <JumbotronSection/>
    <SectionImg/>
    <FooterUp/>
    <FooterCentre/>
    <FooterSocial/>

  </div>
</template>

<script>

import Header from './components/Header.vue';
import FooterUp from './components/FooterUp.vue';
import FooterCentre from './components/FooterCentre.vue';
import FooterSocial from './components/FooterSocial.vue';
import JumbotronSection from './components/JumbotronSection.vue';
import SectionImg from './components/SectionImg.vue';






export default {
  name: 'App',
  components: {
    Header,
    FooterUp,
    FooterCentre,
    FooterSocial,
    JumbotronSection,
    SectionImg
  }
}
</script>

<style lang="scss">
body {
  margin: 0;
}
// #app {
// }
</style>
