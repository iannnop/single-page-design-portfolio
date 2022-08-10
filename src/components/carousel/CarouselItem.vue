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

img {
  width: 270px;
  height: 100%;
  flex: 1 0 100%;
  border-radius: 10px;
}

@media (min-width: 768px) {
  img {
    width: 540px;
  }
}

</style>