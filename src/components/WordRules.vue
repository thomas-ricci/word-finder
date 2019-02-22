<template lang="pug">
.word-rules
  WordRule(v-for="rule in rules" :key="rule.id")
  .new-rule(v-on:click="addRule") + new rule
</template>

<script>

import WordRule from '@/components/WordRule.vue'
export default {
  name: 'wordRules',
  components: {
    WordRule
  },
  data() {
    return {
      rules: []
    }
  },
  methods: {
    addRule() {
      this.rules.push({})
    }
  }
}
</script>

<style lang="stylus">

.word-rules
  width 20em

.new-rule
  margin-top 1em

</style>
