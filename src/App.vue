<template>
  <div id="app">
    <FormGenerator :form="['input[type=text]', 'input[type=email]', 'input[type=button]', 'input[type=text]']" :model="inputData" />
    <p>{{inputData}}</p>
  </div>
</template>

<script>
import FormGenerator from './components/FormGenerator.vue'

export default {
  name: 'App',
  components: {
    FormGenerator
  },
  data(){
    return{
      inputData: []
    }
  }
}
</script>

<style>
#app {
  font-family: Avenir, Helvetica, Arial, sans-serif;
  -webkit-font-smoothing: antialiased;
  -moz-osx-font-smoothing: grayscale;
  text-align: center;
  color: #2c3e50;
}
</style>
