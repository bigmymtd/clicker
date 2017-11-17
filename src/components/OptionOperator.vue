<template>
  <div class="optionOperator">
    <p>オプションA: {{ msg.optionACount }}</p>
    <p>オプションB: {{ msg.optionBCount }}</p>
  </div>
</template>

<script>
export default {
  name: 'OptionOperator',
  data () {
    return {
      msg: window.optionOperator
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

div {
  float: right;
}
</style>
