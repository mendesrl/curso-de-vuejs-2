<template>
  <div id="app">

    <h1>{{ msg }}</h1>

    <test-component></test-component>
    <form-component></form-component>
    <fruit-list-component></fruit-list-component>

  </div>
</template>

<script>
import TestComponent from './components/TestComponent'
import FormComponent from './components/FormComponent'
import FruitListComponent from './components/FruitListComponent'

export default {
  name: 'app',
  data () {
    return {
      msg: 'Curso de Vue'
    }
  },
  components:{
    TestComponent, FormComponent, FruitListComponent
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
}

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
