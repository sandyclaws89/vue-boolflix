<template>
  <div>
      <img 
      :src="FilmCard.poster_path" 
      :alt="FilmCard.original_title"
      >
  </div>
</template>

<script>
export default {
    name: 'CardFilm',
    props:{
      FilmCard: Object,
    }
}
</script>

<style>

</style>