<template>
  <div id="app">
    
    <index></index>
    
  </div>
</template>

<script>
import index from './views/index'

export default {
  components: {
    index,
  }
}
</script>

<style>
html {
  height: 100%;
}

body {
  height: 100%;
  margin: 0;
  padding: 0;
  width: 100%;
  overflow-x: hidden;
}

#app {
  color: #2c3e50;
  margin: 0 auto;
  width: 100%;
  max-width: 540px;
  font-family: Source Sans Pro, Helvetica, sans-serif;
  text-align: center;
}

#app a {
  color: #42b983;
  text-decoration: none;
}

.logo {
  width: 100px;
  height: 100px
}
</style>
