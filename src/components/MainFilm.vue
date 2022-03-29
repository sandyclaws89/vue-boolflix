<template>
  <main class="flex">
       <CardFilm/>
  </main>
</template>

<script>
import CardFilm from './CardFilm.vue'


export default {
    name: 'MainFilm',
    components: {
     CardFilm
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