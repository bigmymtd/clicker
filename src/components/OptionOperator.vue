<template>
  <div class="optionOperator">
      <p>vue: {{ msg }}</p>
      <input v-model="msg">
  </div>
</template>

<script>
export default {
  name: 'OptionOperator',
  data () {
    return {
      msg: 'OptionOperator'
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
