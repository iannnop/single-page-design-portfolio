<script setup>
import HeroSection from './components/HeroSection.vue'
import AboutSection from './components/AboutSection.vue'
import ButtonBlack from './components/ButtonBlack.vue'
import CallToAction from './components/CallToAction.vue';
import WorkSection from './components/WorkSection.vue';
</script>

<template>
  <header>
    <img alt="Vue logo" class="logo" src="./assets/logo.svg" />

    <ButtonBlack />
  </header>

  <main>
    <HeroSection />
    <AboutSection />
    <WorkSection />
    <CallToAction />
  </main>

  <footer>
    <img alt="Vue logo" class="logo" src="./assets/logo.svg" width="64" height="64" />

    <ButtonBlack />
  </footer>
</template>

<style scoped>
header {
  display: flex;
  justify-content: space-between;
  flex-direction: row;
}

main {
  padding: 32px 0;
}

footer {
  display: flex;
  justify-content: space-between;
  flex-direction: row;
}

.logo {
  width: 48px;
  height: 48px;
}

@media (min-width: 1024px) {
  header {
  }
}
</style>
