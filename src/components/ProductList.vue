<template>
    <div class="item">
        <a href="#">
            <div class="image">
                <img :src="productItems.thumb" :alt="productItems.series">
            </div>
            <div class="text">{{ productItems.series }}</div>
        </a>
    </div>
</template>

<script>
export default {
    name: 'ProductList',
    props: {
        productItems: Object
    }
}
</script>

<style lang="scss" scoped>
.item{
    width: calc((100% / 6) - 20px);
    margin-bottom: 50px;

    .image {
        height: 200px;
        // width: 200px;
        overflow-y: hidden;
    }
    

    .text{
        color: lightgrey;
        margin-top: 20px;
        text-transform: uppercase;
    }
}
</style>