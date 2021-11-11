<template>
  <div id="app">
    <div class="container">
      <SiteHeader/>
    </div>
  </div>
</template>

<script>
// import HelloWorld from './components/HelloWorld.vue'
import SiteHeader from './components/SiteHeader.vue'

export default {
  name: 'App',
  components: {
  // HelloWorld
    SiteHeader
  }
}
</script>

<style lang="scss">
/* #app {
  font-family: Avenir, Helvetica, Arial, sans-serif;
  -webkit-font-smoothing: antialiased;
  -moz-osx-font-smoothing: grayscale;
  text-align: center;
  color: #2c3e50;
  margin-top: 60px;
} */
@import './assets/scss/variables.scss';
@import './assets/scss/common.scss';

</style>
