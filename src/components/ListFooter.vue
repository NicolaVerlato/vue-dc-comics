<template>
    <section>
        <div class="container">
            <div class="links">
                <div class="list-item">
                    <h3>DC COMICS</h3>
                    <ul>
                        <li>
                            <a href="#">Characters</a>
                        </li>
                        <li>
                            <a href="#">Comics</a>
                        </li>
                        <li>
                            <a href="#">Movies</a>
                        </li>
                        <li>
                            <a href="#">TV</a>
                        </li>
                        <li>
                            <a href="#">Games</a>
                        </li>
                        <li>
                            <a href="#">Videos</a>
                        </li>
                        <li>
                            <a href="#">News</a>
                        </li>
                    </ul>

                    <div class="list-item shop">
                    <h3>SHOP</h3>
                    <ul>
                        <li>
                            <a href="#">Shop DC</a>
                        </li>
                        <li>
                            <a href="#">Shop DC Collectibles</a>
                        </li>
                    </ul>
                </div>
                </div>

                <div class="list-item">
                    <h3>DC</h3>
                    <ul>
                        <li>
                            <a href="#">Terms Of Use</a>
                        </li>
                        <li>
                            <a href="#">Privacy Policy (New)</a>
                        </li>
                        <li>
                            <a href="#">Ad Choises</a>
                        </li>
                        <li>
                            <a href="#">Advertising</a>
                        </li>
                        <li>
                            <a href="#">Jobs</a>
                        </li>
                        <li>
                            <a href="#">Subscription</a>
                        </li>
                        <li>
                            <a href="#">Talent Workshop</a>
                        </li>
                        <li>
                            <a href="#">CPSC Certificates</a>
                        </li>
                        <li>
                            <a href="#">Ratings</a>
                        </li>
                        <li>
                            <a href="#">Shop Help</a>
                        </li>
                        <li>
                            <a href="#">Contact Us</a>
                        </li>
                    </ul>
                </div>

                <div class="list-item">
                    <h3>SITES</h3>
                    <ul>
                        <li>
                            <a href="#">DC</a>
                        </li>
                        <li>
                            <a href="#">MAD Magazine</a>
                        </li>
                        <li>
                            <a href="#">DC Kids</a>
                        </li>
                        <li>
                            <a href="#">DC Universe</a>
                        </li>
                        <li>
                            <a href="#">CD Power Visa</a>
                        </li>
                    </ul>
                </div>
            </div>

            <div class="image">
                <img src="../assets/img/dc-logo-bg.png" alt="logo">
            </div>
        </div>
    </section>
</template>

<script>
export default {
    name: 'ListFooter'
}
</script>

<style lang="scss" scoped>
section{
    background-image: url(../assets/img/footer-bg.jpg);

    .container{
        display: flex;
        justify-content: space-between;
        position: relative;
        padding: 30px 0;
    }

    .links{
        display: flex;
    }

    .list-item{
        margin-right: 20px;
    }

    .shop{
        margin-top: 20px;
    }

    h3{
        color: white;
        margin-bottom: 8px;
    }

    a{
        color: grey;
        font-size: 12px;
    }

    .image img{
        width: 460px;
        position: absolute;
        top: -80px;
        right: 0;
    }

}
</style>