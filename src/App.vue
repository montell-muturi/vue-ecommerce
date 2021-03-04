<template>
  <div id="app">
    <navbar></navbar>
    <router-view></router-view>
  </div>
</template>

<script>
import Navbar from "./components/Navbar.vue";

export default {
  components: {
    Navbar
  }
}
</script>

<style lang="scss">
@import url('https://fonts.googleapis.com/css2?family=Poppins&family=Raleway&display=swap');
#app{
  height: 100vh;
  font-family: 'Raleway', sans-serif;
}
h1, h2, h3, h4, h5, h6{
  font-family: 'Poppins', sans-serif;
}
</style>
