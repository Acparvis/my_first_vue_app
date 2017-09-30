<template>
  <div class="graph">
    <barchart></barchart>
  </div>
</template>

<script>
  import barchart from './graph.js'
  export default {
    name: 'graph',
    components: {
      barchart
    },
    data () {
      return {
        msg: ''
      }
    },
    props: ['num']
  }
</script>

<style scoped>

</style>
