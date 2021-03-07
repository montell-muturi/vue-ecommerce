<template>
  <div class="product">
      <img src="@/assets/golden-pothos.png" alt="">
      <h3>Potted Aloe Vera</h3>
      <h5>Money</h5>
  </div>
</template>

<script>
export default {
  name: "product",
};
</script>

<style lang="scss" scoped>
.product{
    flex-grow: 1;
    display: flex;
    flex-direction: column;
    border: 1px solid rgba(0, 0, 0, 0.1);
    border-radius: 0.2rem;
    margin: 0.2rem;
    padding: 0 1rem;
    width: 20%;
    transition: box-shadow 0.3s ease-in-out;
}

.product:hover{
    box-shadow: 0.1rem 0.2rem 0.5rem 0 rgba(0, 0, 0, 0.15);
}

.product img{
    width: 100%;
    height: 12rem;
    object-fit: contain;
}
</style>