<template>
  <div id="app">
    <div id="nav">
      <link1></link1>
      <link2></link2>
    </div>
  </div>
</template>

<script>
import input1 from './components/input'
import resultado from './components/resultado'
export default {
  components: {
'link1': input1,
'link2':resultado
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
}
#nav {
  padding: 30px;
}

#nav a {
  font-weight: bold;
  color: #2c3e50;
}

#nav a.router-link-exact-active {
  color: #42b983;
}
</style>
