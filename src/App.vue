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
