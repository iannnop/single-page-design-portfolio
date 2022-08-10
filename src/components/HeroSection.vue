<script>
import SkillGrid from "./SkillGrid.vue";

export default {
  components: {
    SkillGrid
  }
}
</script>

<template>
  <div>
    <h1>Design solutions made easy</h1>
    <p>With over ten years of experience in various design disciplines, I'm your one-stop shop for your design needs.</p>
  </div>
  <SkillGrid />
</template>

<style scoped>
div {
  padding-bottom: 32px;
}

h1 {
  font-size: 36px;
  line-height: 46px;
  font-weight: 700;
  color: var(--black);
  text-align: center;
}

p {
  margin: 16px 0;
  margin-left: auto;
  margin-right: auto;
  width: 80%;
  text-align: center;
}
</style>