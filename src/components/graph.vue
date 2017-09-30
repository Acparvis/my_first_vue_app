<template>
  <div class="graph">
		<h1>Graph</h1>
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
