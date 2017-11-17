<template>
  <div class="employee">
    <p>社員: {{ msg.view }}人</p>
    <button v-on:click="msg.click()"><img src="../assets/employee.png"/></button>
  </div>
</template>

<script>
export default {
  name: 'Employee',
  data () {
    return {
      msg: window.employeesFactory
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
