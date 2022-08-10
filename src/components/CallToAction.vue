<script>
import ButtonColored from "./ButtonColored.vue"

export default {
  components: {
    ButtonColored
  }
}
</script>

<template>
  <div>
    <h2>Book a call with me</h2>
    <p>I'd love to have a chat to see how I can help you. The best first step is for us to discuss your project during a free consultation. Then we can move forward from there.</p>
    <ButtonColored />
  </div>
</template>

<style scoped>
div {
  background-color: var(--black);
  color: var(--light-cream);
  border-radius: 10px;
  padding: 48px 24px;
  text-align: center;
}

p {
  margin: 24px 0;
}
</style>