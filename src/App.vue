<template>
  <div id="app">
    <FileHeader />

    <main>
      <MainContent />
      <ListContent />
    </main>

    <footer>
      <ListFooter />
    </footer>

  </div>
</template>

<script>
// import HelloWorld from './components/HelloWorld.vue'
import FileHeader from './components/FileHeader.vue'
import MainContent from './components/MainContent.vue'
import ListContent from './components/ListContent.vue'
import ListFooter from './components/ListFooter.vue'


export default {
  name: 'App',
  components: {
    // HelloWorld
    FileHeader,
    MainContent,
    ListContent,
    ListFooter
}
}
</script>

<style lang="scss">
@import './style/common'

</style>
