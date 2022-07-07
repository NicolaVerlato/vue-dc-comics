<template>
    <section>
        <div class="container">
            <div class="flag">
                <span>CURRENT SERIES</span>
            </div>

            <div class="product-list">
                <ProductList v-for="product, index in products" :key="index" :productItems="product"/>
            </div>

            <div class="more">
                <a href="#">LOAD MORE</a>
            </div>
        </div>
    </section>
</template>

<script>
import ProductList from './ProductList.vue'
import fileJSON from '../assets/dc-comics.json'

export default {
    name: 'MainContent',
    components: {
        ProductList
    },
    data() {
        return {
            products: fileJSON
        }
    }
}
</script>

<style lang="scss" scoped>
@import '../style/color';
section{
    background-color: $main_color;
    color: white;
    padding-top: 50px;
    padding-bottom: 30px;
    position: relative;

    .product-list{
        display: flex;
        flex-wrap: wrap;
        justify-content: space-around;
    }

    .flag{
        position: absolute;
        top: -20px;
        left: 200px;
        background-color: $secondary_color;
        font-weight: 700;
        font-size: 20px;
        padding: 10px 30px;
    }
    .more {
        text-align: center;

        a{
            color: white;
            background-color: $secondary_color;
            padding: 10px 50px;
            font-weight: 700;
        }
    } 
}
</style>