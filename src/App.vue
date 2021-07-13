<template>
  <div id="app">
    <Navbar />
    <Main :comics="comics" />
    <Footer />
  </div>
</template>

<script>
import Navbar from './components/Navbar.vue'
import Main from './components/Main.vue'
import Footer from './components/Footer.vue'
import comicsJson from './jsons/dc-comics.json'

export default {
  name: 'App',
  components: {
    Navbar,
    Main,
    Footer
  },
  data: function() {
    return {
      comics: comicsJson,
    }
  }
}
</script>

<style lang="scss">
  @import './style/app.scss';
</style>
