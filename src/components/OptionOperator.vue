<template>
  <div class="optionOperator">
    <p>{{msg.optionAName}} 購入数: {{ msg.optionACount }}</p>
    <p>{{msg.optionBName}} 購入数: {{ msg.optionBCount }}</p>
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
</style>
