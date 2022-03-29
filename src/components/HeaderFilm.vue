<template>
  <header class="flex header">
     <div>
         logo
     </div>

     <input
     id="film-id"
     v-model="StrFilm"
     type="text"
     name="film"

     >
  </header>
</template>

<script>

export default {
 name: 'HeaderFilm',
 data() {
     return {
         StrFilm: '',
     }
 },
 methods: {
     debug (console) {
         console.log(@click.console)
     }
 }
}
</script>

<style scoped lang='scss' >
    .header{
        height: 8vh;
        background-color: gray;
        align-items: center;
        justify-content: space-between;
        input{
            width: 200px;
            margin-right: 20px;
            height: 30px;
            
        }
        div{
            margin-left: 20px;
        }
    }

</style>