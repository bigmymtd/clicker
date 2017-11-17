<template>
  <div class="optionView">
    <button v-on:click="msg.purchaseOptionA()">オプションA購入</button>
    <p>オプションA価格: {{ msg.optionAPrice }}</p>
    <button v-on:click="msg.purchaseOptionB()">オプションB購入</button>
    <p>オプションB価格: {{ msg.optionBPrice }}</p>
  </div>
</template>

<script>
export default {
  name: 'OptionView',
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
  border: 1px solid #000000;
  width:400px;
  display: table-cell;
  vertical-align: middle;
}
</style>
