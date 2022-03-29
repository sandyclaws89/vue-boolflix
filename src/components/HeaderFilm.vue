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
     @input="$emit('film-inserted', StrFilm)"

     >
    <button @click="debug(StrFilm)">
        HEADER DEBUG BUTTON
        </button>
    <button>Search</button>
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
     debug (event) {
         console.log(event)
     }

},
}
</script>

<style lang='scss' >
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