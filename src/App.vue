<template>
  <div id="app">
    <img alt="Vue logo" src="./assets/logo.png">
    <HelloWorld msg="Welcome to Your Vue.js App"/>
    <Header/>
    <Main/>
    <Footer/>
  </div>
</template>

<script>
import HelloWorld from './components/HelloWorld.vue';
import Header from './components/macro/Header.vue';
import Main from './components/macro/Main.vue';
import Footer from './components/macro/Footer.vue';

export default {
  name: 'App',
  components: {
    HelloWorld,
    Header,
    Main,
    Footer
  }
}
</script>

<style lang="scss">
#app {
  font-family: Avenir, Helvetica, Arial, sans-serif;
  -webkit-font-smoothing: antialiased;
  -moz-osx-font-smoothing: grayscale;
  text-align: center;
  color: #2c3e50;
  margin-top: 60px;
}
</style>
