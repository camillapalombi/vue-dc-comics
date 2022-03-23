<template>
  <div id="app">
    <HeaderDc />
    <MainDc />
    <MainNavbar />
    <FooterDc />
  </div>
</template>

<script>
import HeaderDc from './components/HeaderDc.vue'
import MainDc from './components/MainDc.vue'
import MainNavbar from './components/MainNavbar.vue'
import FooterDc from './components/FooterDc.vue'




export default {
  name: 'App',
  components: {
    HeaderDc,
    MainDc,
    MainNavbar,
    FooterDc
  }
}
</script>

<style lang="scss">
@import './assets/style/style';
</style>
