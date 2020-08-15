<template>
  <div id="app">
    <Navbar />
    <router-view/>
  </div>
</template>

<script>
import Navbar from './components/Navbar'

export default {

  components: {
    Navbar
  }
  
}
</script>

<style lang="scss">
@import url('https://fonts.googleapis.com/css2?family=Share+Tech&family=Share+Tech+Mono&display=swap');

* {
  margin: 0;
  padding: 0;
  box-sizing: border-box;
  font-family: 'Share Tech', sans-serif;
  background: black;
  color: white;
}


h1, h2, h3, h4 h5, h6 {
  font-family: 'Share Tech Mono', monospace;
}


</style>
