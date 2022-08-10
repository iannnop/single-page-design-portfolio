<script>
import ButtonColored from "./ButtonColored.vue";

export default {
  components: {
    ButtonColored,
  }
}
</script>

<template>
  <div class="container">
    <img src="../assets/image-amy.webp" />
    <div>
      <h2>I'm Amy, and I'd love to work on your next project</h2>
      <p>I love working with others to create beautiful design solutions. I've designed everything from brand illustrations to complete mobile apps. I'm also handy with a camera!</p>    
      <ButtonColored />
    </div>
  </div>
</template>

<style scoped>
img {
  margin: 40px 0;
  width: 300px;
  height: auto;
}

div .container {
  text-align: center;
  margin: 80px 0;
}

p {
  margin: 24px 0; 
}

h2 {
  color: var(--black);
  font-weight: 700;
  font-size: 26px;
  line-height: 33px;
}

</style>