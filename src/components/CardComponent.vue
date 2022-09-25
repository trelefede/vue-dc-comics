<template>
  <div class="card">
    <img :src="comic.thumb" :alt="comic.series">
    <span> {{ comic.series.toUpperCase() }} </span>
  </div>
</template>

<!-- {
    "thumb": "https://www.dccomics.com/sites/default/files/styles/covers192x291/public/comic-covers/2018/09/AC1000_DLX_162-001_HD_5ba13723281ab0.37845353.jpg?itok=ZsI-C5eX",
    "price": "$19.99",
    "series": "Action Comics",
    "type": "comic book"
}, -->

<script>
export default {
    name: "CardComponent",
    props: {
        comic: Object,
    }
}
</script>

<style lang="scss" scoped>
.card{
    display: flex;
    flex-direction: column;
    width: calc(100% / 6 - 20px);
    padding: 0 10px;
    text-align: left;
    color: white;
    font-size: 0.7rem;
    img{
        width: 150px;
        height: 160px;
        padding: 30px 0 10px
    }
}
</style>