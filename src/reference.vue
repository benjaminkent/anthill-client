<template lang="pug">
  .hero-container
    .hero-text
      h1
        | ANTHILL
    .hero-image-container
      img.hero-image(src="../assets/ant-hero.jpeg")
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
  height: 370px;
  padding-top: 50px;
}

.hero-text {
  padding-top: 175px;
  margin: 0;
  position: absolute;
  font-size: 2rem;
}

h1 {
  font-family: "Major Mono Display", monospace;
  text-align: center;
  left: 100px;
  color: #07efb5;
}
</style>

