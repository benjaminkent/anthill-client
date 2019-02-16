<template>
  <div class="header">
    <header class="header">
      <img class="logo" src="../../assets/ant-logo.svg" alt="logo">
      <nav class="big-nav">
        <ul class="nav-list">
          <li class="big-header">
            <a href="#">Home</a>
          </li>
          <li class="big-header">
            <a href="#">About</a>
          </li>
          <li class="big-header">
            <a href="#">in the Hill</a>
          </li>
        </ul>
      </nav>
      <div class="hamburger">
        <div class="hamburger-line"></div>
        <div class="hamburger-line"></div>
        <div class="hamburger-line"></div>
      </div>
    </header>
  </div>
</template>

<script>
export default {
  name: "Header"
};
</script>

<style scoped lang="scss">
@import url("https://fonts.googleapis.com/css?family=Major+Mono+Display");

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
  font-family: "Major Mono Display", monospace;
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
  border: 1px solid #fff;
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