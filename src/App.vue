<template>
  <div id="app">
    <Toggle />
    <img alt="JnS logo" src="./assets/jns-logo-transparent.png">
    <Nav msg="a portfolio"/>
  </div>
</template>

<script>
import Nav from './components/Nav.vue'
import Toggle from './components/Toggle.vue'

export default {
  name: 'App',
  components: {
    Toggle,
    Nav,
  }
}
</script>

<style lang="scss">
html {
  background: #FFF;
  &.dm {
    background: #35373b;
    #app {
      color: #FFF;
    }
    img {
      filter: invert(1);
    }
  }
}
#app {
  color: #2c3e50;
  font-family: Avenir, Helvetica, Arial, sans-serif;
  margin-top: 60px;
  text-align: center;
  -moz-osx-font-smoothing: grayscale;
  -webkit-font-smoothing: antialiased;
}
</style>
