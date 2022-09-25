<template>
  <main>
    <div class="card-container">
      <CardComponent :comic="comic" v-for="comic in cards" :key="comic.series" />
    </div>
    <button>LOAD MORE</button>
  </main>
</template>

<script>
import CardComponent from "./CardComponent.vue"

export default {
    name: 'ContentComponent',
    props: {
      cards: Array,
    },
    components: {
      CardComponent,
    }
}
</script>

<style scoped lang="scss">
@mixin max-width{
    max-width: 1000px;
    margin: 0 auto;
}

main{
  display: flex;
  flex-direction: column;
  justify-content: center;
  background-color: rgb(21, 19, 19);
}

.card-container{
  @include max-width;
  display: flex;
  justify-content: center;
  flex-wrap: wrap;
  margin: 0 auto;
  max-width: 1000px;
}

button{
  background-color: #0182f9;;
  border-style: none;
  padding: 10px 50px;
  margin: 40px auto 15px;
  color: #fff;
  font-weight: bold;
  font-size: 0.8rem;
  flex-shrink: 1;
}
</style>