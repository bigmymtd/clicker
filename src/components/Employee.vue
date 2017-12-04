<template>
  <div class="employee">
    <p>
    <span class="employee_num">
    社員: {{ msg.view }}人
    </span>
    </p>
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
  width:400px;
  display: table-cell;
  vertical-align: middle;
  background-image : url(../assets/kaisya_ayatsuru_joushi.png);
  background-color: #42b983;
  background-size: 10px;

  border-style: solid;
  border-width: 24px 24px 24px 24px;
  -moz-border-image: url(../assets/border.png) 48 48 49 49 round stretch;
  -webkit-border-image: url(../assets/border.png) 48 48 49 49 round stretch;
  -o-border-image: url(../assets/border.png) 48 48 49 49 round stretch;
  border-image: url(../assets/border.png) 48 48 49 49 fill round stretch;
}

.employee_num {
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
