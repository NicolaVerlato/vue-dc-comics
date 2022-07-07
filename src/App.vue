<template>
  <div id="app">
    <header>
      <FileHeader />
    </header>

    <main>
      <FileJumbotron />
      <MainContent />
      <ListContent />
    </main>

    <footer>
      <ListFooter />
      <FooterBottom />
    </footer>

  </div>
</template>

<script>
import FileHeader from './components/FileHeader.vue'
import FileJumbotron from './components/FileJumbotron.vue'
import MainContent from './components/MainContent.vue'
import ListContent from './components/ListContent.vue'
import ListFooter from './components/ListFooter.vue'
import FooterBottom from './components/FooterBottom.vue'


export default {
  name: 'App',
  components: {
    FileHeader,
    FileJumbotron,
    MainContent,
    ListContent,
    ListFooter,
    FooterBottom
}
}
</script>

<style lang="scss">
@import './style/common'

</style>
