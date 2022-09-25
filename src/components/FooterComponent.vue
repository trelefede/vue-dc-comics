<template>
  <footer>
    <LinksFooter />
    <UserComponent />
  </footer>
</template>

<script>
import UserComponent from "./UserComponent.vue";
import LinksFooter from "./LinksFooter.vue";

export default {
    name: 'FooterComponent',
    components: {
        UserComponent,
        LinksFooter,
    }
}
</script>

<style lang="scss" scoped>

</style>