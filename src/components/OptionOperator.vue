<template>
  <div class="optionOperator">
    <p>{{msg.optionAName}} : {{ msg.optionACount }}</p>
    <p>{{msg.optionBName}} : {{ msg.optionBCount }}</p>
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

p {
  border: 3px solid #000000;
  vertical-align: middle;
  background-color: #ffffff;

  border-style: solid;
  border-width: 24px 24px 24px 24px;
  -moz-border-image: url(../assets/border.png) 48 48 49 49 round stretch;
  -webkit-border-image: url(../assets/border.png) 48 48 49 49 round stretch;
  -o-border-image: url(../assets/border.png) 48 48 49 49 round stretch;
  border-image: url(../assets/border.png) 48 48 49 49 fill round stretch;
}
</style>
