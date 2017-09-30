<template>
  <div class="shadow">
		<h1>Shadow {{ num }}</h1>
  </div>
</template>

<script>
  export default {
    name: 'shadow',
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
