<template>
  <header>
        <img src="../assets/dc-logo.png" alt="logo-small">
        <nav>
            <ul>
                <li><a href="#">CHARACTERS</a></li>
                <li><a href="#">COMICS</a></li>
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
    height: 50px;
    padding: 20px 0;
}

ul{
    display: flex;
    list-style-type: none;
    a{
        padding: 20px 10px;
        text-decoration: none;
        color: #2f4f4f;
        font-weight: bold;
        font-size: 0.7rem;
    }
    
}
</style>