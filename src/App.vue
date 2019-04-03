<template>
  <div id="app">
    <v-header :seller="seller"></v-header>
  </div>
</template>

<script>
import qs from 'query-string'
import VHeader from 'components/v-header/v-header'

export default {
  data() {
    return {
      seller: {
        id: qs.parse(location.search).id
      }
    }
  },
  methods: {
  },
  components: {
    VHeader
  }
}
</script>
<style lang="stylus" scoped>
  #app
    .tab-wrapper
      position: fixed
      top: 136px
      left: 0
      right: 0
      bottom: 0
</style>
