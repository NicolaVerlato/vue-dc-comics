<template>
    <section>
        <div class="container">
            <!-- <FileJumbotron /> -->
        </div>
    </section>
</template>

<script>
// import FileJumbotron from './FileJumbotron.vue'

export default {
    name: 'MainContent',
    components: {
        // FileJumbotron
    }
}
</script>

<style lang="scss" scoped>
@import '../style/color';
section{
    background-color: $main_color;
    color: white;
    padding: 40px 0;
}
</style>