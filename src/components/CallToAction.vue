<script>
import ButtonColored from "./ButtonColored.vue"

export default {
  components: {
    ButtonColored
  }
}
</script>

<template>
  <div class="outer">
    <div class="inner">
      <h2>Book a call with me</h2>
      <p>I'd love to have a chat to see how I can help you. The best first step is for us to discuss your project during a free consultation. Then we can move forward from there.</p>
    </div>
    <ButtonColored />
  </div>
</template>

<style scoped>
div .outer {
  background-color: var(--black);
  color: var(--light-cream);
  border-radius: 10px;
  padding: 48px 24px;
  text-align: center;
}

h2 {
  font-weight: 700;
  font-size: 26px;
  line-height: 32px;
}

p {
  margin: 24px 0;
}

@media (min-width: 768px) {
  div .outer {
    padding: 56px 75px;
  }

  h2 {
    font-size: 32px;
    line-height: 40px;
  }

  p {
    font-size: 18px;
    line-height: 28px;
    margin: 26px 0;
  }
}

@media (min-width: 1440px) {
  div .outer {
    display: flex;
    text-align: left;
  }

  div .inner {
    margin-right: auto;
    width: 540px;
  }

  h2 {
    font-size: 40px;
    line-height: 50px;
  }

  p {
    font-size: 18px;
    line-height: 28px;
    margin: 26px 0 0 0;
  }
}
</style>