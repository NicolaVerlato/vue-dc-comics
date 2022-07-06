<template>
    <section>
        <div class="container">
            <ul>
                <li v-for="element, index in mainList" :key="index" :class="{'underline': element.underline}">
                    <img :src="element.imgSrc" :alt="element.text">
                    <a :href="element.link">{{element.text}}</a>
                </li>
            </ul>
        </div>
    </section>
</template>

<script>
export default {
    name: 'ListContent',
    data() {
        return{
            mainList: [
                {
                    link: '#',
                    text: 'DIGITAL COMICS',
                    imgSrc: require('../assets/img/buy-comics-digital-comics.png')
                },
                {
                    link: '#',
                    text: 'DC MERCHANDISE',
                    imgSrc: require('../assets/img/buy-comics-merchandise.png')
                },
                {
                    link: '#',
                    text: 'SUBSCRIPTION',
                    imgSrc: require('../assets/img/buy-comics-subscriptions.png')
                },
                {
                    link: '#',
                    text: 'COMIC SHOP LOCATOR',
                    imgSrc: require('../assets/img/buy-comics-shop-locator.png')
                },
                {
                    link: '#',
                    text: 'DC POWER VISA',
                    imgSrc: require('../assets/img/buy-dc-power-visa.svg')
                }
            ]
        }
    }
}
</script>

<style lang="scss" scoped>
@import '../style/color';
section{
    background-color: $secondary_color;
    color: white;
    padding: 40px 0;
    position: relative;
    z-index: 10;

    ul{
        display: flex;
        justify-content: space-around;

        li{
            display: flex;
            align-items: center;
        }

        img{
            width: 40px;
            margin-right: 10px;
        }

        a{
            color: white;
            font-size: 12px;
        }
    }
}
</style>