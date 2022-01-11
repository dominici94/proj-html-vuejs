<template>
  <div id="app">
    <Header/>
    <Jumbotron/>
    <Main/>
    <Footer/>
  </div>
</template>

<script>
import Header from './components/macro/Header.vue';
import Jumbotron from './components/sections/Jumbotron.vue';
import Main from './components/macro/Main.vue';
import Footer from './components/macro/Footer.vue';

export default {
  name: 'App',
  components: {
    Header,
    Jumbotron,
    Main,
    Footer
  }
}
</script>

<style lang="scss">
@import './assets/style/global.scss';
// @import './assets/style/partials/variables.scss';

</style>
