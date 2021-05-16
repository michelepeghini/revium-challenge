<template>
  <div id="nav" class="nav sticky">
    <router-link class="nav__link" to="/">Link 1</router-link>
    <router-link class="nav__link" to="/">Link 2</router-link>
    <router-link class="nav__link" to="/">Link 3</router-link>
  </div>
</template>

<style scoped lang="stylus">
.nav {
  text-align: center;
  margin: 0;
  padding: 20px 0;
  border: 1px solid green;
  height: 70px;
  background-color: white;

  &__link {
    padding: 5px 15px;
    border-radius: 20px;
    border: 1px solid green;
    margin: 0 10px;
    font-size: 20px;
    color: green;
    vertical-align: -webkit-baseline-middle;

    &:hover {
      color: white;
      background-color: green;
    }
  }
}

.sticky {
  position: fixed;
  top: 0;
  width: 100%;
  z-index: 99999;
}
</style>
