<template>
  <div id="app">
    <v-header></v-header>
    <v-content></v-content>
    <v-footer></v-footer>
    <router-view></router-view>
  </div>
</template>

<script>
  import VHeader from './components/header'
  import VFooter from './components/footer'
  import VContent from './components/content'

  export default {
    components: {
        VHeader,
        VFooter,
        VContent
    }
  }
</script>

<style>

</style>
