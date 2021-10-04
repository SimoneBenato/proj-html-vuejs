<template>
  <div id="app">
    <Header/>
    <Wrapper/>
    <Component1/>
    <Component2/>
    <Component3/>
    <Component4/>
    <Component5/>
    <Footer/>
  </div>
</template>

<script>
import Header from './components/Header.vue'
import Wrapper from './components/Wrapper.vue'
import Component1 from './components/Component1.vue'
import Component2 from './components/Component2.vue'
import Component3 from './components/Component3.vue'
import Component4 from './components/Component4.vue'
import Component5 from './components/Component5.vue'
import Footer from './components/Footer.vue'

export default {
  name: 'App',
  components: {
    Header,
    Wrapper,
    Component1,
    Component2,
    Component3,
    Component4,
    Component5,
    Footer
  }
}
</script>

<style lang="scss">
@import 'styles/generals.scss';
@import 'styles/colors.scss';
@import '~@fortawesome/fontawesome-free/css/all.min.css';
</style>
