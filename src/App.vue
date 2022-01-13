<template>
  <div id="app">
    <Header :info="navbar"/>
    <Jumbotron/>
    <Main/>
    <Footer :info="navbar"/>
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
    Footer,
  },
  data() {
    return {
      navbar: [
        'Recipes',
        'Places',
        'Blog',
        'About',
        'Contact'
      ]
    }  
  },
  
}
</script>

<style lang="scss">
@import './assets/style/global.scss';
// @import './assets/style/partials/variables.scss';

</style>
