<template>
  <div id="app">
    <Header/>
    <router-view/>
    <Footer/>
  </div>
</template>

<script>
import Header from './views/Header.vue'
import Footer from './views/Footer.vue'
export default {
  name: 'app',
  components:{
    Header,
    Footer,
  }
}
</script>

<style>
#app {
  -webkit-font-smoothing: antialiased;
  -moz-osx-font-smoothing: grayscale;
  text-align: center;
  color: #2c3e50;
}

*{
  font-family: 'Cormorant Garamond', serif;
}

#nav {
  padding: 30px;
}

#nav a {
  color: #707070;
}

#nav a:hover{
  text-decoration: none;
}

#nav a.router-link-exact-active {
  color: #b9b9b9;
}
</style>
