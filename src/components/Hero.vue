<template lang="pug">
  .hero-container
    .hero-text
      h2.hero-welcome
        | welcome, to the
      h1.hill
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
  height: 290px;
  background-position: center center;
  background-size: cover;
  width: 100vw;
  z-index: -1000;
}

.hero-text {
  padding-top: 95px;
  margin: 0;
  position: absolute;
  display: flex;
  flex-direction: column;
  align-items: center;
}

h2 {
  font-family: "Major Mono Display", monospace;
  font-size: 1.5rem;
  color: #07efb5;
  margin-bottom: 140px;
}

h1 {
  font-family: "Major Mono Display", monospace;
  font-size: 4rem;
  text-align: center;
  left: 100px;
  color: #07efb5;
  margin: 0;
}
</style>

