<template>
  <div id="app">
    <HeaderComponent />
    <JumbotronComponent />
    <ContentComponent :cards="comics" />
    <BuyComponent />
    <FooterComponent />
  </div>
</template>

<script>
import HeaderComponent from "./components/HeaderComponent.vue";
import JumbotronComponent from "./components/JumbotronComponent.vue";
import ContentComponent from "./components/ContentComponent.vue";
import BuyComponent from "./components/BuyComponent.vue";
import FooterComponent from "./components/FooterComponent.vue";

import { comics } from "./data/data.js";

export default {
  name: 'App',
  data(){
    return {
      comics,
    }
  },
  components: {
    HeaderComponent,
    JumbotronComponent,
    ContentComponent,
    BuyComponent,
    FooterComponent,
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
