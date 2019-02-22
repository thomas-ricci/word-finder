<template lang="pug">
.home
  header
    h1 Word Finder
  main
    WordRules
    ResultsList
</template>

<script>
// @ is an alias to /src
import WordRules from '@/components/WordRules.vue'
import ResultsList from '@/components/ResultsList.vue'

export default {
  name: 'home',
  components: {
    WordRules,
    ResultsList
  }
}
</script>

<style lang="stylus">

header
  width 100%
  margin-bottom 5em

main
  display flex
</style>
