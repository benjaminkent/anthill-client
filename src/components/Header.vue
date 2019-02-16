<template lang="pug">
  .header-container
    TopHeader
    PopOutMenu
</template>

<script>
import TopHeader from "./header/TopHeader"
import PopOutMenu from "./header/PopOutMenu"

export default {
  name: "Header",
  components: {
    TopHeader,
    PopOutMenu
  }
}
</script>

<style lang="scss">
@import url("https://fonts.googleapis.com/css?family=Major+Mono+Display");

.header-container {
  font-family: "Major Mono Display", monospace;
}
</style>

