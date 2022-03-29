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

<style scoped lang="scss">
  div{
    width: 200px;
    height: 250px;
    background-color: burlywood;
    img {
      width: 150px;
      height: 200px
    }
  }
  
</style>