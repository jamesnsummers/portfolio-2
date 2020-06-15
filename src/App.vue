<template>
  <div id="app">
    <Toggle />
    <img alt="JnS logo" src="./assets/jns-logo-transparent.png">
    <Nav msg="a portfolio"/>
    <Body />
  </div>
</template>

<script>
import Nav from './components/Nav.vue'
import Toggle from './components/Toggle.vue'
import Body from './components/Body.vue'

export default {
  name: 'App',
  components: {
    Toggle,
    Nav,
    Body,
  }
}
</script>

<style lang="scss">
html {
  background: #FFFFFF;
  img {
    height: 150px;
    filter: invert(15%);
    width: auto;
  }
  &.dm {
    background: #35373B;
    #app {
      color: #FFFFFF;
    }
    img {
      filter: invert(1);
    }
  }
}
#app {
  color: #2C3E50;
  font-family: Avenir, Helvetica, Arial, sans-serif;
  margin-top: 60px;
  text-align: center;
  -moz-osx-font-smoothing: grayscale;
  -webkit-font-smoothing: antialiased;
}
</style>
