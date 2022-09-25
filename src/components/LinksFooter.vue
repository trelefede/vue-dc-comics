<template>
  <footer>
    <div class="container">
        <!-- column 1 -->
        <div>
            <div>
                <h3>DC COMICS</h3>
                <UL>
                    <li><a href="#">Characters</a></li>
                    <li><a href="#">Comics</a></li>
                    <li><a href="#">Movies</a></li>
                    <li><a href="#">TV</a></li>
                    <li><a href="#">Games</a></li>
                    <li><a href="#">VIdeos</a></li>
                    <li><a href="#">News</a></li>
                </UL>
            </div>
            <div>
                <h3>SHOP</h3>
                <ul>
                    <li><a href="#">Shop DC</a></li>
                    <li><a href="#">Shop DC Collectibles</a></li>
                </ul>
            </div>
        </div>

        <!-- column 2 -->
        <div>
            <h3>DC</h3>
            <UL>
                <li><a href="#">Characters</a></li>
                <li><a href="#">Comics</a></li>
                <li><a href="#">Movies</a></li>
                <li><a href="#">TV</a></li>
                <li><a href="#">Games</a></li>
                <li><a href="#">VIdeos</a></li>
                <li><a href="#">News</a></li>
            </UL>
        </div>

        <!-- column 3 -->
        <div>
            <h3>SITES</h3>
            <ul>
                <li><a href="#">DC</a></li>
                <li><a href="#">MAD Magazine</a></li>
                <li><a href="#">DC Kids</a></li>
                <li><a href="#">DC Universe</a></li>
                <li><a href="#">DC Power Visa</a></li>
            </ul>
        </div>
        <div id="logo-footer">
            <img src="../assets/dc-logo-bg.png" alt="logo-bg">
        </div>
    </div>
  </footer>
</template>

<script>
export default {
    name: "LiknsFooter",
}
</script>

<style lang="scss" scoped>
@mixin max-width{
    max-width: 1000px;
    margin: 0 auto;
}

footer{
    position: relative;
    background-image: url(../assets/footer-bg.jpg)
}

.container{
    @include max-width;
    display: flex;
    align-items: stretch;
    justify-content: flex-start;
    > div{
    padding: 40px 30px 40px 0;
    }   
}

h3{
    color: #fff;
    font-weight: bolder;
    margin: 13px 0;
    }

ul{
    list-style-type: none;
    a{
        padding-top: 10px; 
        text-decoration: none;
        color: #7a7a7a;
        font-weight: bold;
        font-size: 0.9rem;
    }
}

#logo-footer{
    img{
        width: 50%;
        position: absolute;
        top: -92px;
        right: 53px;
    }
}
</style>