<template>
  <div id="app">
    <Weather />
  </div>
</template>


<script>
import Weather from './components/people.vue'
export default {
  name: 'app',
  components: {
    Weather
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
table {
  font-family: arial, sans-serif;
  border-collapse: collapse;
  width: 100%;
  border-spacing: 0;
}

td, th {
  border: 1px solid #dddddd;
  text-align: left;
  padding: 10px;
  /* display: block */
}
.ID{
  width: 40%
}
.NAME{
  width: 20%
}
.ATT{
  width: 20%
}
.VIP{
  width: 20%
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
