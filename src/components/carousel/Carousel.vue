<script>
import CarouselItem from "./CarouselItem.vue"

export default {
  components: {
    CarouselItem,
},
  data() {
    return {
      slides: [
        "src/assets/image-slide-4.jpg",
        "src/assets/image-slide-5.jpg",
        "src/assets/image-slide-1.jpg",
        "src/assets/image-slide-2.jpg",
        "src/assets/image-slide-3.jpg",
        "src/assets/image-slide-4.jpg",
        "src/assets/image-slide-5.jpg",
        "src/assets/image-slide-1.jpg",
        "src/assets/image-slide-2.jpg",
      ],
      slideIndex: 0,
      slideWidth: window.innerWidth >= 768 ? 570 : 285
    }
  },
  created() {
  window.addEventListener("resize", this.calculateSlide);
  },
  destroyed() {
  window.removeEventListener("resize", this.calculateSlide);
  },
  methods: {
    moveSlide(direction) {
      if (Math.abs(this.slideIndex + direction) > 2) {
        this.slideIndex *= -1
      } else {
        this.slideIndex += direction
      }
    },
    calculateSlide(e) {
      this.slideWidth = window.innerWidth >= 768 ? 570 : 285
    }
  },
}
</script>

<template>
  <div class="carousel"
    :style="{ 
      transform: `translateX(${-slideIndex * (slideWidth)}px)`
    }"
    @transitionend="adjustSlide()"
  >
    <div class="carousel-inner">
      <CarouselItem v-for="(slide, index) in slides" :slide="slide" />
    </div>
  </div>
  <button @mousedown="moveSlide(-1)">
    <img src="../../assets/icon-arrow-left.svg" />
  </button>
  <button @mousedown="moveSlide(1)">
    <img src="../../assets/icon-arrow-right.svg" />
  </button>
</template>

<style scoped>
.carousel {
  margin: 32px 0;
}

.carousel-inner {
  display: flex;
  justify-content: center;
  gap: 15px;
}

button {
  width: 64px;
  height: 64px;
  margin: 0 8px;
  background-color: var(--black);
  border-radius: 100%;
  border: none;
}

button:hover {
  background-color: var(--galactic-blue);
  cursor: pointer;
}

@media (min-width: 768px) {
  .carousel {
    margin: 56px 0;
  }

  .carousel-inner {
    gap: 30px;
  }
}
</style>