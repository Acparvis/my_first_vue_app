<template>
  <div class="graph">
		<h1>Graph</h1>
    <thing></thing>
  </div>
</template>

<script>
  import thing from './graph.js'
  export default {
    name: 'graph',
    componenets: {
      thing
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
