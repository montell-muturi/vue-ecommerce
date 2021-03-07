<template>
  <div class="products">
    <div class="container">
      <h1>Fan Faves</h1>
      <div class="products-wrapper">
        <product></product>
        <product></product>
        <product></product>
        <product></product>
        <product></product>
        <product></product>
      </div>
    </div>
  </div>
</template>

<script>
import Product from "../components/Product.vue";

export default {
  name: "products",
  components: { Product },
};
</script>

<style lang="scss" scoped>
.products h1 {
  font-weight: 100;
}

.products-wrapper{
  display: flex;
  flex-wrap: wrap;
}
</style>