<template>
  <div id="app">
    <FileHeader />

    <main>
      <MainContent />
      <ListContent />
    </main>

  </div>
</template>

<script>
// import HelloWorld from './components/HelloWorld.vue'
import FileHeader from './components/FileHeader.vue'
import MainContent from './components/MainContent.vue'
import ListContent from './components/ListContent.vue'

export default {
  name: 'App',
  components: {
    // HelloWorld
    FileHeader,
    MainContent,
    ListContent
}
}
</script>

<style lang="scss">
@import './style/common'

</style>
