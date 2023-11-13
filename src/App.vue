<script>

import NavBar from './components/NavBar.vue';
import Footer from './components/Footer.vue';
import Main from './components/Main.vue'


export default {
  components: {
    NavBar,
    Footer,
    Main,
  },
  data() {
    return {
    }
  }
}

</script>

<template>
  <NavBar/>
  <Main/>
  <Footer/>
</template>

<style lang="scss">
@use './styles/general.scss';
</style>
