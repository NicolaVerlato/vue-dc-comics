<template>
    <section>
        <div class="container">
            <div class="btn">
                <a href="#">SIGN-UP NOW!</a>
            </div>

            <ul>
                <li class="blue">
                    <a href="#">
                        FOLLOW US
                    </a>
                </li>
                <li>
                    <a href="#">
                        <img src="../assets/img/footer-facebook.png" alt="facebook">
                    </a>
                </li>
                <li>
                    <a href="#">
                        <img src="../assets/img/footer-twitter.png" alt="twitter">
                    </a>
                </li>
                <li>
                    <a href="#">
                        <img src="../assets/img/footer-youtube.png" alt="youtube">
                    </a>
                </li>
                <li>
                    <a href="#">
                        <img src="../assets/img/footer-pinterest.png" alt="pinterest">
                    </a>
                </li>
                <li>
                    <a href="#">
                        <img src="../assets/img/footer-periscope.png" alt="periscope">
                    </a>
                </li>
            </ul>
        </div>
    </section>
</template>

<script>
export default {
    name: 'FooterBottom'
}
</script>

<style lang="scss" scoped>
@import '../style/color';
section{
    background-color: #303030;
    padding: 30px;
    position: relative;
    z-index: 12;

    .container{
        display: flex;
        justify-content: space-between;
        align-items: center;
    }

    .btn{
        border: 2px solid $secondary_color;
        padding: 10px;

        a{
            color: white;
            font-size: 13px;
        }
    }

    ul{
        display: flex;
        align-items: center;
    }

    li{
        padding: 0 10px;
    }
    .blue a{
        color: $secondary_color;
        font-weight: 700;
    }

    a img{
        width: 30px;
    }
}
</style>