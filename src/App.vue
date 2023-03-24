<template>
  <div id="app">
    <Navbar/>
    <Content/>
    <Footer/>
    <!-- <HelloWorld msg="Welcome to Your Vue.js App"/> -->
  </div>
</template>

<script>
import Content from './components/Content.vue'
import Navbar from './components/Navbar.vue'
import Footer from './components/Footer.vue';

export default {
  name: 'App',
  components: {
    Content,
    Navbar,
    Footer
  }
}
</script>

<style>

html, body {
  margin:0;
  padding:0;
  height:100%;
}

#app {
  /* height: 100vh;
  width: 100vw; */
  font-family: Avenir, Helvetica, Arial, sans-serif;
  -webkit-font-smoothing: antialiased;
  -moz-osx-font-smoothing: grayscale;
  /* text-align: center; */
  /* color: #2c3e50; */
  /* margin-top: 60px; */
}
</style>
