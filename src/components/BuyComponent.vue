<template>
  <div class="container">
    <div>
    <div>
        <img src="../assets/buy-comics-digital-comics.png" alt="DIGITAL-COMICS">
        <a href="#">DIGITAL COMICS</a>
    </div>
    <div>
        <img src="../assets/buy-comics-merchandise.png" alt="DC MERCHANDISE">
        <a href="#">DC MERCHANDISE</a>
    </div>
    <div>
        <img src="../assets/buy-comics-subscriptions.png" alt="SUBSCRIPTION">
        <a href="#">SUBSCRIPTION</a>
    </div>
    <div>
        <img src="../assets/buy-comics-shop-locator.png" alt="COMIC SHOP">
        <a href="#">COMIC SHOP</a>
    </div>
    <div>
        <img src="../assets/buy-dc-power-visa.svg" alt="DC POWER VISA">
        <a href="#">DC POWER VISA</a>
    </div>
</div>
  </div>
</template>

<script>
export default {
    name: 'BuyComponent',
}
</script>

<style scoped lang="scss">
$color: white;

@mixin max-width{
    max-width: 1000px;
    margin: 0 auto;
}
.container{
    background-color: #0182f9;
    >div{
        @include max-width;
        display: flex;
        justify-content: space-around;
        div{
            display: flex;
            align-items: center;
            color: $color;
            img{
                width: 40px;
                height: auto;
                padding: 30px 10px 30px 0;
            }
            a{
                font-size: 0.6rem;
                text-decoration: none;
                font-weight: bold;
                color: $color;
            }
        }
    }
}

</style>