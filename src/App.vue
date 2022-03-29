<template>

  <div id="app">
    <HeaderFilm
    @film-inserted="setFilmSearch"
    />
     <button @click="debug(strSearchFilm)">
        APP DEBUG BUTTON
        </button>
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
  },
  data() {
    return {
      strSearchFilm: '',
    }
  },
  methods: {
    setFilmSearch(filmArgument) {
      this.strSearchFilm = filmArgument;
    },
     debug (event) {
         console.log(event)
     }
  }
}
</script>

<style lang="scss">
@import './assets/styles/style.scss';


</style>
