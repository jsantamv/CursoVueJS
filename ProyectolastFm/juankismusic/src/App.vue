<template lang="pug">
#app
  img(src='./assets/logo.png')
  h1 JUANKISMUSIC
  ul
    li (v-for="artist in artists"){{
      artist.name    }}

</template>

<script>
export default {
  name: 'app',
  data () {
    return {
      artists: [
        { name: 'David Bowie' },
        { name: 'daft punk' },
        { name: 'Red Hot Chill Peppers' },
        { name: 'AC DC' }
      ]
    }
  }
}
</script>

<style lang="stylus" >
#app
  font-family 'Avenir', Helvetica, Arial, sans-serif
  -webkit-font-smoothing antialiased
  -moz-osx-font-smoothing grayscale
  text-align center
  color green !important
  margin-top 60px

h1, h2
  font-weight normal

ul
  list-style-type none
  padding 0

li
  display inline-block
  margin 0 10px

a
  color #42b983
</style>
