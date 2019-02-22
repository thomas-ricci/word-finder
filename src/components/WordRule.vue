<template lang="pug">
.rule
  select(v-on:change="optionChanged")
    option(v-for="option in options" v-bind:value="option.id") {{ option.title }}
  input(type="text")
</template>

<script>
export default {
  name: 'WordRule',
  data() {
    return {
      options: [
        {
          id: 'starts_with',
          title: 'Starts with',
        },
        {
          id: 'ends_with',
          title: 'Ends with'
        }
      ]
    }
  },
  methods: {
    optionChanged() {
      console.log('Option changed!');
    }
  }
}
</script>

<style lang="stylus" scoped>
input[type="text"]
  width 5em
  margin-left 1em
</style>
