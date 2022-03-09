<template>
  <div id="app">
    <HeaderComics/>
    <JumbotronComics/>
    <IconsComics/>
  </div>
</template>

<script>
import HeaderComics from './components/HeaderComics.vue'
import JumbotronComics from './components/JumbotronComics.vue'
import IconsComics from './components/IconsComics.vue'

export default {
  name: 'App',
  components: {
    HeaderComics,
    JumbotronComics,
    IconsComics
  }
}
</script>

<style lang="scss">
* {
  font-family: Arial, Helvetica, sans-serif;
  margin: 0;
  padding: 0;
  box-sizing: border-box;
}
</style>
