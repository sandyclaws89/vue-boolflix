<template>
  <main class="flex">
       <CardFilm
        v-for="film in arrFilm"
        :key="film.original_title"
        :FilmCard="film" 
       />
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
 }

}
</script>

<style scoped lang='scss'>
    main{
        height: 92vh;
        background-color: royalblue;
        justify-content: center;
        align-items: center;
    }
</style>