<template lang="pug">
  .header-container
    header.header
      img.logo(src="@/assets/ant-logo.svg" alt="logo")
      nav.big-nav
        ul.nav-list
          li.big-header
            a(href="#")
              | Home
          li.big-header
            a(href="#")
              | About
          li.big-header
            a(href="#")
              | in the Hill
      .hamburger(v-on:click="hide = !hide")
        .hamburger-line
        .hamburger-line
        .hamburger-line
    .pop-menu(:class="{ hide: hide }")
      p.pop-menu-x(v-on:click="hide = !hide")
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
  name: "Header",
  data: function () {
    return {
      hide: true
    }
  }
};
</script>

<style scoped lang="scss">
@import url("https://fonts.googleapis.com/css?family=Major+Mono+Display");

.header-container {
  font-family: "Major Mono Display", monospace;
}

.logo {
  height: 2.5rem;
  margin: 2rem 0 1.5rem 1rem;
}

.header {
  position: fixed;
  width: 100%;
  background-color: black;
  color: white;
  box-shadow: 0px 0.5px 5px black;
  z-index: 2;
  display: flex;
  justify-content: space-between;
}

.nav-list {
  list-style-type: none;
  display: flex;
  margin: 2.5rem 0 0 0;
  padding: 0;
  justify-content: space-around;

  a {
    color: #59E0FF;
    text-decoration: none;
    font-size: 1.3rem;
  }
}

.big-header {
  margin: 0 1rem;
}

.hamburger {
  margin: 35px 20px 35px 0;
  cursor: pointer;
}

.hamburger-line {
  border: 1px solid #59E0FF;
  width: 25px;
  margin: 5px;
}

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

.hide {
  margin-right: -100%;
}

@media (max-width: 500px) {
  .big-header {
    display: none;
  }
}

@media(min-width: 501px) {
  .hamburger {
    display: none;
  }
}

@media (min-width: 600px) {
  .big-header {
    margin: 0 1.7rem;
  }
}
</style>