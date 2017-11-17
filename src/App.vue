<template>
  <div id="app">
    <Employee/>
    <OptionView/>
    <OptionOperator/>
  </div>
</template>

<script>
import Employee from './components/Employee'
import OptionView from './components/OptionView'
import OptionOperator from './components/OptionOperator'

export default {
  name: 'app',
  components: {
    Employee,
    OptionView,
    OptionOperator
  }
}
</script>

<style>
#app {
  font-family: 'Avenir', Helvetica, Arial, sans-serif;
  -webkit-font-smoothing: antialiased;
  -moz-osx-font-smoothing: grayscale;
  text-align: center;
  color: #2c3e50;
  margin-top: 60px;
  background-image : url(assets/logo.png);
}
</style>
