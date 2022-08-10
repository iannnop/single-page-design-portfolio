<script>
import Carousel from "./carousel/Carousel.vue";

export default {
  components: {
    Carousel
  }
}
</script>

<template>
  <div>
    <h2>My Work</h2>
    <Carousel />
  </div>
</template>

<style scoped>
h2 {
  color: var(--black);
  font-size: 24px;
  line-height: 30px;
  font-weight: 700;
}

div {
  margin: 100px 0;
  text-align: center;
}
</style>