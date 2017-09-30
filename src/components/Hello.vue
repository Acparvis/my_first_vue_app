<template>
  <div class="hello">
    <h1>{{ number }}</h1>
    <button @click="doMath"> Press me! </button>
    <p>{{ watchMath }}</p>
    <Shadow :num="number"
    ></Shadow>
    <input></input>
    <Graph></Graph>
  </div>
</template>

<script>
import Shadow from './shadow.vue'
import Graph from './graph.vue'
export default {
  name: 'hello',
  components: {
    Shadow,
    Graph
  },
  data () {
    return {
      msg: 'Welcome to Your Vue.js App',
      number: 2
    }
  },
  methods: {
    doMath: function () {
      this.number += 2
    }
  },
  computed: {
    watchMath: function () {
      if (this.number > 10) {
        return 'Greater than 10!'
      }
    }
  }
}
</script>

<!-- Add "scoped" attribute to limit CSS to this component only -->
<style scoped>
h1, h2 {
  font-weight: normal;
}

ul {
  list-style-type: none;
  padding: 0;
}

li {
  display: inline-block;
  margin: 0 10px;
}

a {
  color: #42b983;
}
</style>
