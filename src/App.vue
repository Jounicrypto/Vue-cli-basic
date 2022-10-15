<template>
  <div id="app">
    <nav>
      <router-link to="/">Houses</router-link> |
      <router-link to="/about">About</router-link>
    </nav>
    <router-view/>
  </div>
</template>

<style lang="scss">
#app {
  font-family: Avenir, Helvetica, Arial, sans-serif;
  text-align: center;
  text-decoration: none;
}

nav {
  padding: 30px;

  a {
    font-weight: bold;
    color: #000;
    text-decoration: none;

    &.router-link-exact-active {
      // color: #42b983;
      text-decoration: none;
    }
  }
}
</style>
