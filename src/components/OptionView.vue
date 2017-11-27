<template>
  <div class="optionView">
    <div class="A_button">
    <button v-on:click="msg.purchaseOptionA()" style="width:100%;"><img src="../assets/animalface_kirin.png" width="100"/><span class="A_text"><font size="5" line-height=100px>オプションA価格: {{ msg.optionAPrice }}</font></span> </button>
    </div>
    <div class="B_button">
    <button v-on:click="msg.purchaseOptionB()" style="width:100%;"><img src="../assets/animalface_kirin.png" width="100"/><span class="A_text"><font size="5" line-height=100px>オプションB価格: {{ msg.optionBPrice }}</font></span> </button>
    </div>
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
  border: 10px solid #000000;
  width:400px;
  display: table-cell;
  vertical-align: middle;
  background-color: #42b983;
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
