<template lang="pug">
  .pop-menu
    p.pop-menu-x
      | X
    nav
      ul
        li.link
          | Home
        li.link
          | About
        li.link
          | in the Hill
</template>

<script>
export default {
  name: "PopOutMenu"
}
</script>

<style lang="scss" scoped>
.pop-menu {
  position: fixed;
  right: 0;
  width: 75%;
  top: 0;
  height: 100%;
  background-color: #000;
  color: #59E0FF;
  opacity: 0.93;
  z-index: 3;
  transition: 0.4s ease-in-out;

  .pop-menu-x {
    position: absolute;
    right: 1.5rem;
    font-size: 1.8rem;
    margin-top: 32px;
    margin-right: 4px;
    cursor: pointer;
    color: #59E0FF;
  }

  nav {
    margin-top: 6.5rem;

    li {
      list-style: none;
      font-size: 1.5rem;
      padding: 1.5rem 0;
    }
  }
}
</style>


