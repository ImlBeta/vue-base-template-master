<template>
  <div id="app">
    <Navbar />
    <router-view/>

  </div>
</template>

<script>
import Navbar from '@/containers/NavBar.vue';

export default {
  name: 'RootApp',
  components: {
    Navbar
  }
};
</script>

<style>
body{
  margin: 0px;
  padding: 0px;
}
#app {
  font-family: Avenir, Helvetica, Arial, sans-serif;
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

h1{
  text-align: left;
  font-size: 2em;
}

</style>
