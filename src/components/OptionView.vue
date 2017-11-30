<template>
  <div class="optionView">
    <button v-on:click="msg.purchaseOptionA()" v-bind:disabled="canPurchaseOptionA">{{msg.optionAName}} 購入</button>
    <p>{{msg.optionAName}} 価格: {{ msg.optionAPrice }}</p>
    <button v-on:click="msg.purchaseOptionB()" v-bind:disabled="canPurchaseOptionB">{{msg.optionBName}} 購入</button>
    <p>{{msg.optionBName}} 価格: {{ msg.optionBPrice }}</p>
  </div>
</template>

<script>
export default {
  name: 'OptionView',
  data () {
    return {
      msg: window.optionOperator,
      emp: window.emp
    }
  },
  computed: {
    canPurchaseOptionA () {
      return this.emp.value < this.msg.optionAPrice
    },
    canPurchaseOptionB () {
      return this.emp.value < this.msg.optionBPrice
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
