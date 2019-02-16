<template lang="pug">
  //- .pop-menu.hide
  //-   p.pop-menu-x
  //-     | X
  //-   nav
  //-     ul
  //-       li.link
  //-         | Home
  //-       li.link
  //-         | About
  //-       li.link
  //-         | in the Hill
</template>

<template>
  <div class="pop-menu">
    <p class="pop-menu-x">X</p>
    <nav>
      <ul>
        <li class="link">Home</li>
        <li class="link">About</li>
        <li class="link">in the Hill</li>
      </ul>
    </nav>
  </div>
</template>


<script>
export default {
  name: "PopOutMenu",
  data: function () {
    return {
      hide
    }
  }
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

.hide {
  margin-right: -100%;
}
</style>


