<template>
  <div id="app">
    <div class="main-wrapper">
      <v-header></v-header>
      <v-content></v-content>
      <v-footer></v-footer>
      <router-view></router-view>
    </div>
  </div>
</template>

<script>
  import VHeader from './components/header'
  import VFooter from './components/footer'
  import VContent from './components/content'
  import $ from 'jquery'

  export default {
    components: {
      VHeader,
      VFooter,
      VContent
    },
    mounted () {}
  }
</script>

<style lang="stylus">
  .main-wrapper
    background: #444 url('./assets/banner.jpg')
    background-attachment: fixed
    background-repeat: no-repeat
    background-size: cover
    background-position: center center
    animation: image-wrapper-opacity 1s linear
</style>
