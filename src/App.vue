<template>
  <div id="app">
    <Header/>
    <Wrapper/>
    <Footer/>
  </div>
</template>

<script>
import Header from './components/Header.vue'
import Wrapper from './components/Wrapper.vue'
import Footer from './components/Footer.vue'

export default {
  name: 'App',
  components: {
    Header,
    Wrapper,
    Footer
  }
}
</script>

<style lang="scss">
@import 'styles/generals.scss';
@import 'styles/colors.scss';
@import '~@fortawesome/fontawesome-free/css/all.min.css';
</style>
