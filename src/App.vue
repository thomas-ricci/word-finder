<template lang="pug">
  #app
    //- #nav
    //-   router-link(to="/") Home |
    //-   router-link(to="/about") About
    router-view
</template>

<style lang="stylus">

#app
  font-family 'ISO v0.5', Monospace
  color #000000
  padding 5em
  font-size 12px

h1, h2, h3, h4, h5, h6
  font-size 1.2em

// #nav
//   padding 30px
//   a
//     font-weight bold
//     router-link-exact-active
//       color #42b983
</style>
