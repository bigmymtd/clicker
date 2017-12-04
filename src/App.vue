<template>
  <div id="app">
  <h1>Clicker</h1>
    <Employee/>
    <OptionOperator/>
    <OptionView/>
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
  background-image : url(cow1_animated_128.gif);
  overflow:auto;
  height:600px;
}
</style>
