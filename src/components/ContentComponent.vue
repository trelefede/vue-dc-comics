<template>
  <main>
    <div>--> Content goes here --</div>
  </main>
</template>

<script>
export default {
    name: 'ContentComponent',
}
</script>

<style scoped lang="scss">
@mixin max-width{
    max-width: 1000px;
    margin: 0 auto;
}
main{
    background-color: rgb(21, 19, 19);
    div{
        @include max-width;
        display: flex;
        color: white;
        align-items: center;
        justify-content: center;
        height: 200px;
    }
}
</style>