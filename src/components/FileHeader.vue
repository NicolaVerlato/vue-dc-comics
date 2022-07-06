<template>
    <header>
        <div class="container">
            <div class="logo">
                <img src="../assets/img/dc-logo.png" alt="DC Logo">
            </div>
            <div class="header-list">
                <ul>
                    <li v-for="element, index in headerList" :key="index" :class="{'underline': element.underline}">
                        <a :href="link">{{element.text}}</a>
                    </li>
                </ul>
            </div>
        </div>
    </header>
</template>

<script>
export default {
    name: 'FileHeader',
    data() {
        return{
            headerList: [
                {
                    link: '#',
                    text: 'CHARACTERS',
                    underline: false
                },
                {
                    link: '#',
                    text: 'COMICS',
                    underline: true
                },
                {
                    link: '#',
                    text: 'MOVIES',
                    underline: false
                },
                {
                    link: '#',
                    text: 'TV',
                    underline: false
                },
                {
                    link: '#',
                    text: 'GAMES',
                    underline: false
                },
                {
                    link: '#',
                    text: 'COLLECTIBLES',
                    underline: false
                },
                {
                    link: '#',
                    text: 'VIDEOS',
                    underline: false
                },
                {
                    link: '#',
                    text: 'FANS',
                    underline: false
                },
                {
                    link: '#',
                    text: 'NEWS',
                    underline: false
                },
                {
                    link: '#',
                    text: 'SHOP',
                    underline: false
                }
            ]
        }
    }
}
</script>

<style lang="scss" scoped>
@import '../style/color';

header{
    height: 80px;
    padding-top: 20px;
}
.container{
    display: flex;
    justify-content: space-between;
    line-height: 80px;

    .logo{
        width: 80px;
    }
    .header-list ul{
        display: flex;
    }
    li{
        padding: 10px;
        font-size: 12px;

        &.underline{
            color: $secondary_color;
            border-bottom: 4px solid $secondary_color;
        }
    }
    li{
        color: $main_color;
    }
}
</style>