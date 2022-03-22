<template>
  <div id="app">
    <HeaderDc />
    <MainDc />
    <MainNavbar />
  </div>
</template>

<script>
import HeaderDc from './components/HeaderDc.vue'
import MainDc from './components/MainDc.vue'
import MainNavbar from './components/MainNavbar.vue'
import "./assets/style/style.scss";


export default {
  name: 'App',
  components: {
    HeaderDc,
    MainDc,
    MainNavbar
  }
}
</script>

<style>

</style>
