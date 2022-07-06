<template>
  <div id="app">
    <FileHeader />

  </div>
</template>

<script>
// import HelloWorld from './components/HelloWorld.vue'
import FileHeader from './components/FileHeader.vue'

export default {
  name: 'App',
  components: {
    // HelloWorld
    FileHeader
  }
}
</script>

<style lang="scss">
@import './style/common'

</style>
