<template>
  <div id="app">
    <HeaderComponent />
    <ContentComponent />
    <BuyComponent />
  </div>
</template>

<script>
import HeaderComponent from "./components/HeaderComponent.vue";
import ContentComponent from "./components/ContentComponent.vue";
import BuyComponent from "./components/BuyComponent.vue"

export default {
  name: 'App',
  components: {
    HeaderComponent,
    ContentComponent,
    BuyComponent,
  }
}
</script>

<style lang="scss">
*{
  margin: 0;
  padding: 0;
}
#app {
  font-family: Avenir, Helvetica, Arial, sans-serif;
  -webkit-font-smoothing: antialiased;
  -moz-osx-font-smoothing: grayscale;
}
</style>
