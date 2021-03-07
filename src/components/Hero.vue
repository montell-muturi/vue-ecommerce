<template>
  <div class="hero">
    <div class="glide">
      <div class="glide__track" data-glide-el="track">
        <ul class="glide__slides">
          <li class="glide__slide">
            <img class="slider-image" src="@/assets/slider-1.jpg" alt="" />
            <div class="intro-slider">
              <h1>SUCCULENTS<br>HUB</h1>
            </div>
          </li>
          <li class="glide__slide">
            <img class="slider-image" src="@/assets/slider-2.jpg" alt="" />
          </li>
          <li class="glide__slide">
            <img class="slider-image" src="@/assets/slider-3.jpg" alt="" />
          </li>
        </ul>
      </div>
      <div class="glide__arrows" data-glide-el="controls">
        <button class="glide__arrow glide__arrow--left" data-glide-dir="<">
          prev
        </button>
        <button class="glide__arrow glide__arrow--right" data-glide-dir=">">
          next
        </button>
      </div>
    </div>
  </div>
</template>

<script>
import Glide, { Controls } from "@glidejs/glide";

var sliders = document.querySelectorAll(".glide");

for (var i = 0; i < sliders.length; i++) {
  var glide = new Glide(sliders[i],{
    type: 'carousel',
    animationDuration: 5000,
    autoplay: 4500,
    focusAt: '1',
    startAt: 1,
    perView: 1
  });
  glide.mount({ Controls });
}

export default {
  name: "hero",
};
</script>

<style lang="scss" scoped>
@import "node_modules/@glidejs/glide/src/assets/sass/glide.core";
@import "node_modules/@glidejs/glide/src/assets/sass/glide.theme";

.slider-image {
  height: 30rem;
  width: 100%;
  object-fit: cover;
}

.glide__slide{
  position: relative;
}

.intro-slider{
  position: absolute;
  display: flex;
  top: 0;
  left: 0;
  height: 100%;
  width: 100%;
  justify-content: center;
  align-items: center;
}

.intro-slider > h1{
  text-align: right;
  font-size: 6em;
  font-weight: 900;
  -webkit-text-stroke: 3px #fff;
  -webkit-text-fill-color: transparent;
}
</style>