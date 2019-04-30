<template>
  <div id="app">
    <div id="nav">
      
      <!--chamando os componenetes-->
      
	  <evento1 v-on="numero1" @input="soma">
      </evento1>
      
      <evento2 v-on="numero2" v-bind:numero1="3">
      </evento2>
    
    </div>
  </div>
</template>

<script>

//importa os arquivos dos componentes

import input1 from './components/input'
import resultado from './components/resultado'
import func from '../vue-temp/vue-editor-bridge';

export default {
  
  //delcara os componentes
  components: {

	'evento1': input1,
	'evento2':resultado
},

  //declara os metodos
  methods: {
		
	soma (a, b) {
		return a + b;
	}
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