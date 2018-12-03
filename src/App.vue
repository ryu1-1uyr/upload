<template>
  <div id="app">
    <Editer></Editer>
  </div>
</template>

<script>
import Editer from './components/Editor'

export default {
  name: 'App',
  components: {
    Editer
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
</style>
