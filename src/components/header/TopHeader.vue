<template lang="pug">
  header.header
    img.logo(src="../../assets/ant-logo.svg" alt="logo")
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
    .hamburger
      .hamburger-line
      .hamburger-line
      .hamburger-line
</template>

<script>
export default {
  name: "Header"
};
</script>

<style scoped lang="scss">
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