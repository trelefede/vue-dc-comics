<template>
  <header>
        <img src="../assets/dc-logo.png" alt="logo-small">
        <nav>
            <ul>
                <li><a href="#">CHARACTERS</a></li>
                <li><a href="#" class="active">COMICS</a></li>
                <li><a href="#">MOVIES</a></li>
                <li><a href="#">TV</a></li>
                <li><a href="#">GAMES</a></li>
                <li><a href="#">COLLECTIBLES</a></li>
                <li><a href="#">VIDEOS</a></li>
                <li><a href="#">FANS</a></li>
                <li><a href="#">NEWS</a></li>
                <li><a href="#">SHOP</a></li>
            </ul>
        </nav>
  </header>
</template>

<script>
export default {
    name: 'HeaderComponent',
}
</script>

<style scoped lang="scss">
@mixin max-width{
    max-width: 1000px;
    margin: 0 auto;
}

header{
    @include max-width;
    display: flex;
    justify-content: space-between;
    align-items: center;
}

img{
    width: 50px;
    padding: 10px 0;
}

ul{
    display: flex;
    list-style-type: none;
    height: 100%;
    li{
        padding: 0px 10px;
        height: 100%;
    }
    a{
        text-decoration: none;
        color: #2f4f4f;
        font-weight: bold;
        font-size: 0.7rem;
        height: 100%;
        &.active{
        border-bottom: 3px solid #0182f9;
        color: #0182f9;
        border-bottom-width: 70%;
        }
    }
    
}
</style>