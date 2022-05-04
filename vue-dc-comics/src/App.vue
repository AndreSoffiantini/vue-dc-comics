<template>
  <div id="app">
    <!-- <img alt="Vue logo" src="./assets/logo.png">
    <HelloWorld msg="Welcome to Your Vue.js App"/> -->

  <SiteHeader/>

  <SiteMain/>

  <SiteFooter/>

  </div>
</template>

<script>
//import HelloWorld from './components/HelloWorld.vue'
import SiteHeader from './components/HeaderComponent.vue'
import SiteMain from './components/MainComponent.vue'
import SiteFooter from './components/FooterComponent.vue'

export default {
  name: 'App',
  components: {
    //HelloWorld
    SiteHeader,
    SiteMain,
    SiteFooter,
  }
}
</script>

<style lang="scss">

@import '@/assets/sass/_common';
@import '@/assets/sass/_utilities';
/* @import '@/assets/sass/_variables'; */
@import '@/assets/sass/_grid_structure';

</style>
