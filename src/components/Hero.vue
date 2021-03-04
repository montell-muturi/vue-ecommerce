<template>
  <div class="hero">
    <img src="@/assets/hero-image.jpg" alt="" width="50%" height="100%" />
    <div class="hero-side-content">
      <h1>Succulent Hub</h1>
      <p>
        Lorem ipsum dolor sit, amet consectetur adipisicing elit. Qui et, eaque
        repellat, distinctio natus placeat, totam voluptate aliquam optio
        obcaecati blanditiis dolorem ullam nobis culpa asperiores ipsa quia sunt
        pariatur.
      </p>
    </div>
  </div>
</template>

<script>
export default {
  name: "hero",
};
</script>

<style lang="scss" scoped>
.hero {
  display: flex;
  height: 100vh;

}

.hero-side-content {
  width: 50%;
  padding: 5rem;
}

img {
  object-fit: cover;
}
</style>