<template>
  <footer>
    <div class="container">
        <div>
            <button>SIGN-UP NOW</button>
        </div>
        <div id="social">
            <span>FOLLOW US</span>
            <img src="@/assets/footer-facebook.png" alt="facebook">
            <img src="@/assets/footer-twitter.png" alt="twitter">
            <img src="@/assets/footer-youtube.png" alt="youtube">
            <img src="@/assets/footer-pinterest.png" alt="pinterest">
            <img src="@/assets/footer-periscope.png" alt="periscope">
        </div>
    </div>
  </footer>
</template>

<script>
export default {
    name: "UserComponent",
}
</script>

<style lang="scss" scoped>
@mixin max-width{
    max-width: 1000px;
    margin: 0 auto;
}

footer{
  background-color: #303030;
}

.container{
    @include max-width;
    display: flex;
    align-items: center;
    justify-content: space-between;   
    > div{
        padding: 30px 0;
    }
}

button{
    background-color: #303030;
    border-style: none;
    border: 2px solid #0182f9;
    padding: 12px;
    color: #fff;
    font-weight: bold;
    font-size: 1rem;
}

#social{
    display: flex;
    align-items: center;
    span{
        color: #0182f9;
        font-weight: bold;
        padding: 0 20px;
    }
    img{
        margin-right: 15px;
    }
}
</style>