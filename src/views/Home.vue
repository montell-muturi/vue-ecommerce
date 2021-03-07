<template>
  <div class="home">
    <navbar></navbar>
    <hero></hero>
    <products></products>
  </div>
</template>

<script>
import Hero from '../components/Hero.vue';
import Navbar from '../components/Navbar.vue';
import Products from '../components/Products.vue';

export default {
  components: { Hero, Navbar, Products },
};
</script>

<style lang="scss" scoped>
</style>

