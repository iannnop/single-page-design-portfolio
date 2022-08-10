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
    <div class="text-container">
      <h2>I'm Amy, and I'd love to work on your next project</h2>
      <p>I love working with others to create beautiful design solutions. I've designed everything from brand illustrations to complete mobile apps. I'm also handy with a camera!</p>    
      <ButtonColored />
    </div>
  </div>
</template>

<style scoped>
img {
  width: 300px;
  height: auto;
}

div .container {
  text-align: center;
  margin: 100px 0;
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

@media (min-width: 768px) {
  img {
    translate: -70px;
  }

  div .container {
    text-align: left;
    margin: 120px 0;
    display: flex;
    align-items: center;
  }

  h2 {
    font-size: 32px;
    line-height: 40px;
  }
}

@media (min-width: 1440px) {
  .text-container {
    margin-left: 125px;
    width: 540px;
  }

  img {
    width: 445px;
    translate: 0px;
  }

  div .container {
    max-width: 100%;
    text-align: left;
    margin-left: auto;
    display: flex;
    align-items: center;
  }

  h2 {
    font-size: 40px;
    line-height: 50px;
  }

  p {
    margin: 32px 0;
  }
}

</style>