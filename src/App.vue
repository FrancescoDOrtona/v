<script>

import NavBar from './components/NavBar.vue';
import Footer from './components/Footer.vue';


export default {
  components: {
    NavBar,
    Footer,
  },
  data() {
    return {
    }
  }
}

</script>

<template>
  <NavBar/>
  <Footer/>
</template>

<style lang="scss">
@use './styles/general.scss';
</style>
