<template>
<section class="carousel" aria-label="Gallery">
  <ol class="carousel__viewport">
    <li id="carousel__slide1"
        tabindex="0"
        class="carousel__slide">
      <div class="carousel__snapper">
         <slide1 />
        <a href="#carousel__slide4"
           class="carousel__prev"></a>
        <a href="#carousel__slide2"
           class="carousel__next"></a>
      </div>
    </li>
    <li id="carousel__slide2" tabindex="0" class="carousel__slide">
      <div class="carousel__snapper">
        <slide2 />
      </div>
      <a href="#carousel__slide1"
         class="carousel__prev"></a>
      <a href="#carousel__slide3"
         class="carousel__next"></a>
    </li>
    <li id="carousel__slide3"
        tabindex="0"
        class="carousel__slide">
      <div class="carousel__snapper"><slide3 /></div>
      <a href="#carousel__slide2"
         class="carousel__prev"></a>
      <a href="#carousel__slide4"
         class="carousel__next"></a>
    </li>
    <li id="carousel__slide4"
        tabindex="0"
        class="carousel__slide">
      <div class="carousel__snapper"><slide4 /></div>
      <a href="#carousel__slide3"
         class="carousel__prev"></a>
      <a href="#carousel__slide1"
         class="carousel__next"></a>
    </li>
  </ol>
  <aside class="carousel__navigation">
    <ol class="carousel__navigation-list">
      <li class="carousel__navigation-item">
        <a href="#carousel__slide1"
           class="carousel__navigation-button">Go to slide 1</a>
      </li>
      <li class="carousel__navigation-item">
        <a href="#carousel__slide2"
           class="carousel__navigation-button">Go to slide 2</a>
      </li>
      <li class="carousel__navigation-item">
        <a href="#carousel__slide3"
           class="carousel__navigation-button">Go to slide 3</a>
      </li>
      <li class="carousel__navigation-item">
        <a href="#carousel__slide4"
           class="carousel__navigation-button">Go to slide 4</a>
      </li>
    </ol>
  </aside>
</section>
</template>
<script>
import slide1 from './slide1.vue'
import slide2 from './slide2.vue'
import slide3 from './slide3.vue'
import slide4 from './slide4.vue'

export default {
 components:{
   slide1,
   slide2,
   slide3,
   slide4
 }
}
</script>


<style scoped>
  /*  */
    @keyframes tonext {
  75% {
    left: 0;
  }
  95% {
    left: 100%;
  }
  98% {
    left: 100%;
  }
  99% {
    left: 0;
  }
}

@keyframes tostart {
  75% {
    left: 0;
  }
  95% {
    left: -300%;
  }
  98% {
    left: -300%;
  }
  99% {
    left: 0;
  }
}

@keyframes snap {
  96% {
    scroll-snap-align: center;
  }
  97% {
    scroll-snap-align: none;
  }
  99% {
    scroll-snap-align: none;
  }
  100% {
    scroll-snap-align: center;
  }
}

body {
  max-width: 1920px;
  margin: 0 auto;
  padding: 0 0rem;
  font-family: 'Lato', sans-serif;
}



*::-webkit-scrollbar {
  width: 0;
}


ol, li {
  list-style: none;
  margin: 0;
  padding: 0;
}

.carousel {
  position: relative;
  padding-top: 70vh;
  filter: drop-shadow(0 0 10px #0003);
}

.carousel__viewport {
  position: absolute;
  top: 0;
  right: 0;
  bottom: 0;
  left: 0;
  display: flex;
  overflow: hidden;
  counter-reset: item;
  scroll-behavior:smooth;
  scroll-snap-type:x mandatory;
}

.carousel__slide {
  position: relative;
  flex: 0 0 100%;
  width: 100%;
  background-color: #abc;
  counter-increment: item;
}

.carousel__slide:nth-child(1) {
  background-color: #abc;
}

.carousel__slide:nth-child(2) {
    background-color: #abc;
}
.carousel__slide:nth-child(3) {
     background-color: #abc;
}
.carousel__slide:nth-child(4) {
   background-color: #abc;
}

.carousel__slide:before {
  /* content: counter(item); */
  position: absolute;
  top: 50%;
  left: 50%;
  transform: translate3d(-50%,-40%,70px);
  color: #fff;
  font-size: 2em;
}

.carousel__snapper {
  position: absolute;
  top: 0;
  left: 0;
  width: 100%;
  height: 100%;
  scroll-snap-align: center;
}

@media (hover: hover) {
  .carousel__snapper {
    animation-name: tonext, snap;
    animation-timing-function:linear;
    animation-duration: 2s;
    animation-iteration-count: infinite;
  }

  .carousel__slide:last-child .carousel__snapper {
    animation-name: tostart, snap;
  }
}

@media (prefers-reduced-motion: reduce) {
  .carousel__snapper {
    animation-name: none;
  }
}

.carousel:hover .carousel__snapper,
.carousel:focus-within .carousel__snapper {
  animation-name: none;
}

.carousel__navigation {
  position: absolute;
  right: 0;
  bottom: 0;
  left: 0;
  text-align: center;
}

.carousel__navigation-list,
.carousel__navigation-item {
  display: inline-block;
}

.carousel__navigation-button {
  display: inline-block;
  width: 4.5rem;
  height: 2rem;
  background-clip: content-box;
  border: 0.25rem solid transparent;
  border-radius: 30%;
  font-size: 0;
  transition: transform 0.1s;
}

.carousel::before,
.carousel::after,
.carousel__prev,
.carousel__next {
  position: absolute;
  top: 0;
  margin-top: 0%;
  width: 4rem;
  height: 4rem;
  transform: translateY(-50%);
  border-radius: 50%;
  font-size: 0;
  outline: 0;
}

.carousel::before,
.carousel__prev {
  left: -1rem;
}

.carousel::after,
.carousel__next {
  right: -1rem;
}

.carousel::before,
.carousel::after {

  z-index: 1;
  background-size: 1.5rem 1.5rem;
  background-repeat: no-repeat;
  background-position: center center;
  color: #fff;
  font-size: 2.5rem;
  line-height: 4rem;
  text-align: center;
  pointer-events: none;
}

</style>