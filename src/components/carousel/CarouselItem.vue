<script>
export default {
  props: ["slide", "currentSlide", "index"],
}
</script>

<template>
  <div class="carousel-item">
    <img :src="slide"/>
  </div>
</template>

<style scoped>
.carousel-item {
}

img {
  width: 270px;
  height: 100%;
  flex: 1 0 100%;
  border-radius: 10px;
}
</style>