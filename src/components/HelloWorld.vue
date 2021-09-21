<template>
  <h1>{{ count }}</h1>
  <button @click="incrementCount()" >Increment Count</button>
  <button @click="decrementCount()">Decrement Count</button>
</template>

<script>
export default {
  name: 'HelloWorld',
  methods: {
    incrementCount: function() {
      this.count++;
    },
    decrementCount: function() {
      this.count--;
    }
  },
  data: function () {
    return {
      count: 0
    }
  },
}
</script>

<!-- Add "scoped" attribute to limit CSS to this component only -->
<style scoped>
h3 {
  margin: 40px 0 0;
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
