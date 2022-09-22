<template>
  <div id="app">
    <HeaderComponent />
  </div>
</template>

<script>
import HeaderComponent from "./components/HeaderComponent.vue";

export default {
  name: 'App',
  components: {
    HeaderComponent,
  }
}
</script>

<style lang="scss">
#app {
  font-family: Avenir, Helvetica, Arial, sans-serif;
  -webkit-font-smoothing: antialiased;
  -moz-osx-font-smoothing: grayscale;
}
</style>
