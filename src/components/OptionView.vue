<template>
  <div class="optionView">
    <div class="A">
      <div class="A_button">
      <button v-on:click="msg.purchaseOptionA()">オプションA購入<img src="../assets/animalface_kirin.png" width="100"/></button>
      </div>
    <p>
    オプションA価格: {{ msg.optionAPrice }}
    </p>
    </div>
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
  border: 10px solid #000000;
  width:400px;
  display: table-cell;
  vertical-align: middle;
  background-color: #ff0000;
}

.A{
  border: 3px solid #000000;
  vertical-align: middle;
  font-size: 10px;
  background-image : url(../assets/animalface_kirin.png);
  background-color: #42b983;
  background-size: 100px;
}

.A_button{
  border: 3px solid #000000;
  vertical-align: middle;
  font-size: 20px;
  background-color: #ffffff;
}
</style>
