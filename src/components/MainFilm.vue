<template>
  <main class="flex">
       <CardFilm
        v-for="film in arrFilm.result"
        :key="film.original_title"
        :FilmCard="film" 
       />




        <button @click="debug(film)">
        MAIN DEBUG BUTTON
        </button>
  </main>
</template>

<script>
// /* eslint-disable */
import CardFilm from './CardFilm.vue';
import axios from 'axios';


export default {
    name: 'MainFilm',
    components: {
     CardFilm
 },
    data() {
    return{
        arrFilm: null,
     } 
    },
    props: {
        strSearchFilm: String,
    },
    created() {
    axios.get('https://api.themoviedb.org/3/search/movie?api_key=93fea60e6afb40367324d80ed28c9dd4&query=ritorno+al+futuro')
      .then(axiosResponse => {
        this.arrFilm = axiosResponse.result;
        // this.$emit('data-arrived', this.arrDischi);
      })
    },
     methods: {
     debug (event) {
         console.log(event)
     }
    },
    computed: {
        findedFilm() {
            return this.arrFilm.filter()
        },
    }

}
</script>

<style lang='scss'>
    main{
        height: 92vh;
        background-color: royalblue;
        justify-content: center;
        align-items: center;
    }
</style>