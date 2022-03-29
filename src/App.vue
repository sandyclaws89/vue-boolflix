<template>
  <div id="app">
    <HeaderFilm/>
    <MainFilm/>
  </div>
</template>

<script>
import HeaderFilm from './components/HeaderFilm.vue'
import MainFilm from './components/MainFilm.vue'


export default {
  // 93fea60e6afb40367324d80ed28c9dd4 CHIAVE API
  name: 'App',
  components: {
    HeaderFilm,
    MainFilm
  }
}
</script>

<style lang="scss">
@import './assets/styles/style.scss';


</style>
