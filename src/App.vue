<template>
  <div id="app">
    <div id="nav">
      <router-link to="/"><IconLogo /></router-link>
      <div id="nav-items">
        <router-link to="/">Home</router-link>
        <router-link to="/about">About</router-link>
        <router-link to="/projects">Projects</router-link>
      </div>
    </div>
    <router-view/>
  </div>
</template>

<script>
import IconLogo from '@/components/icons/IconLogo.vue'

export default {
  components: {
    IconLogo
  }
}
</script>

<style lang="scss">

$theme-white: #fdfffc;
$theme-blue: #235789;
$theme-yellow: #f1d302;
$theme-red: #c1292e;
$theme-black: #020100;

$default-padding: 30px;

#app {
  font-family: Avenir, Helvetica, Arial, sans-serif;
  -webkit-font-smoothing: antialiased;
  -moz-osx-font-smoothing: grayscale;
  color: $theme-blue;
}

#nav {
  background-color: $theme-white;
  padding: $default-padding;
  #nav-items {
    float: right;
    a {
    font-weight: bold;
    color: #2c3e50;
    padding: $default-padding;

      &.router-link-exact-active {
        color: $theme-red;
      }
    }
  }
}

svg {
  width: 350px;
  margin: right;
}
</style>
