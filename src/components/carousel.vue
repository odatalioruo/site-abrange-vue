<template>
<section class="carousel">
  <div class="slides">
    <div class="slides-item slide-1" id="slide-1">1</div>
    <div class="slides-item slide-2" id="slide-2">2</div>
    <div class="slides-item slide-3" id="slide-3">3</div>
    <div class="slides-item slide-4" id="slide-4">4</div>
    <div class="slides-item slide-5" id="slide-5">5</div>       
  </div>
  <div class="carousel__nav">
    <a class="slider-nav" href="#slide-1">1</a>
    <a class="slider-nav" href="#slide-2">2</a>
    <a class="slider-nav" href="#slide-3">3</a>
    <a class="slider-nav" href="#slide-4">4</a>
    <a class="slider-nav" href="#slide-5">5</a>
  </div>
</section>
</template>

<style scoped>
body {
  font-family: sans-serif;
}

.carousel {
  margin: 0 auto;
  overflow: hidden;
  text-align: center;
}

.slides {
  display: flex;
}

.slides-item {
  align-items: center;
  border-radius: 10px;
  display: flex;
  flex-shrink: 0;
  font-size: 100px;
  height: 600px;
  justify-content: center;
  margin: 0 1rem;
  position: relative;
  transform: scale(1);
  transform-origin: center center;
  transition: transform .5s;
  width: 100%;
}

.carousel__nav {
  padding: 1.25rem .5rem;
}

.slider-nav {
  align-items: center;
  background-color: #ddd;
  border-radius: 50%;
  color: #000;
  display: inline-flex;
  height: 1.5rem;
  justify-content: center;
  padding: .5rem;
  position: relative;
  text-decoration: none;
  width: 1.5rem;
}

.slider-nav:hover,
.slider-nav:active {
  background-color: #000;
  color: #fff;
}

.slide-1 {
  background: url('./img/topo.png');
  background-size: cover;
}

.slide-2 {
  background-color: #bfd;
}

.slide-3 {
  background-color: #cdf;
}

.slide-4 {
  background-color: #dca;
}

.slide-5 {
  background-color: #ffc;
}
</style>