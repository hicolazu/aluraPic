<template>
  <div id="app">
    <h1>{{ msg }}</h1>

    <ul> 
        <li v-for="foto of fotos"> 
          <img :src="foto.url" :alt="foto.titulo">
        </li>
    </ul>
  </div>
</template>

<script>
export default {
  name: 'app',
  data () {
    return {
      msg: 'Welcome to Alura Pic',
      fotos: [
      {
          url: '../foto.jpg',
          titulo: 'cachorro'
      },
      {
        url: '../foto2.jpg',
        titulo: 'tucano'
      }]
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
