<template>
  <div class="optionView">
    <div class="A_button">
    <button v-on:click="msg.purchaseOptionA()" style="width:100%;" v-bind:disabled="canPurchaseOptionA"><img src="../assets/animalface_kirin.png" width="100" align="left"/><span class="A_text"><font size="5" line-height=100px>{{msg.optionAName}} ¥{{ msg.optionAPrice }}</font></span> </button>
    </div>
    <div class="B_button">
    <button v-on:click="msg.purchaseOptionB()" style="width:100%;" v-bind:disabled="canPurchaseOptionB"><img src="../assets/animalface_kirin.png" width="100" align="left"/><span class="A_text"><font size="5" line-height=100px>{{msg.optionBName}} ¥{{ msg.optionBPrice }}</font></span> </button>
    </div>
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

div {
  border: 10px solid #000000;
  width:400px;
  display: table-cell;
  vertical-align: middle;

  border-style: solid;
  border-width: 24px 24px 24px 24px;
  -moz-border-image: url(../assets/border.png) 48 48 49 49 round stretch;
  -webkit-border-image: url(../assets/border.png) 48 48 49 49 round stretch;
  -o-border-image: url(../assets/border.png) 48 48 49 49 round stretch;
  border-image: url(../assets/border.png) 48 48 49 49 fill round stretch;
}

.A_button{
  border: 3px solid #000000;
  vertical-align: middle;
  background-color: #ffffff;
  display: block;
}

.B_button{
  border: 3px solid #000000;
  vertical-align: middle;
  background-color: #ffffff;
  display: block;
}
</style>
