<script>
</script>

<template>
  <div class="grid">
    <div class="grid-item graphic-design">
      <img src="../assets/pattern-graphic-design.svg"/>
      <p class="grid-text">Graphic Design</p>
    </div>
    <div class="grid-item ui-ux">
      <img src="../assets/pattern-ui-ux.svg"/>
      <p class="grid-text">UI/UX</p>
    </div>
    <div class="grid-item apps">
      <img src="../assets/pattern-apps.svg"/>
      <p class="grid-text">Apps</p>
    </div>
    <div class="grid-item illustrations">
      <img src="../assets/pattern-illustrations.svg" />
      <p class="grid-text">Illustrations</p>
    </div>
    <div class="grid-item photography">
      <img src="../assets/pattern-photography.svg" />
      <p class="grid-text">Photography</p>
    </div>
    <div class="grid-item motion-graphics">
      <img src="../assets/pattern-motion-graphics.svg" />
      <p class="grid-text">Motion Graphics</p>
    </div>
  </div>
</template>

<style scoped>

img {
  margin-left: auto;
  align-self: center;
}

.grid {
  display: grid;
  grid-template-columns: 2;
  grid-template-rows: repeat(6, 182px) ;
  grid-template-areas: 
  'a a'
  'a a'
  'b c'
  'd d'
  'e e'
  'f f';
  gap: 24px;
}

.grid-item {
  display: flex;
  flex-direction: column;
  justify-content: space-between;
  flex: 1;
  padding: 24px;
  border-radius: 8px;
}

.graphic-design {
  grid-area: a;
  background-color: var(--galactic-blue);
}

.ui-ux {
  grid-area: b;
  background-color: var(--summer-yellow);
}

.apps {
    grid-area: c;
  background-color: var(--pink);
}

.illustrations {
  grid-area: d;
  background-color: var(--light-red);
}

.photography {
  grid-area: e;
  background-color: var(--cyan);
}

.motion-graphics {
  grid-area: f;
  background-color: var(--violet);
}

.grid-text {
  color: #FFFFFF;
  font-size: 24px;
}
</style>