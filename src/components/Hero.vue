<template lang="pug">
  .hero-container
    .hero-text
      h1
        | ANTHILL
    .hero-image
</template>


<script>
export default {
  name: "Hero"
}
</script>

<style lang="scss" scoped>
.hero-container {
  display: flex;
  flex-direction: column;
  align-items: center;
}

.hero-image {
  padding-top: 100px;
  background: url("../assets/ant-hero.jpeg");
  height: 330px;
  background-position: center center;
  background-size: cover;
  width: 100vw;
  z-index: -1000;
}

.hero-text {
  padding-top: 175px;
  margin: 0;
  position: absolute;
}

h1 {
  font-family: "Major Mono Display", monospace;
  font-size: 4rem;
  text-align: center;
  left: 100px;
  color: #07efb5;
  z-index: 1000;
}
</style>

