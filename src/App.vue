<template>
  <Home />
</template>

<script>
import Home from './Home.vue'

export default {
  name: 'App',
  components: {
    Home    
  }
}
</script>

<style>
* {
  margin: 0;
  padding: 0;
  box-sizing: border-box;
}

body {
  min-height: 100vh;
}

@font-face {
  font-family: goudy;
  src: url("./assets/Goudy_Bookletter_1911/GoudyBookletter1911-Regular.ttf");
}

#app {
  font-family: goudy;
  -webkit-font-smoothing: antialiased;
  -moz-osx-font-smoothing: grayscale;
  text-align: center;
  color: #2c3e50;
}

.row {
  display: flex;
  flex-direction: row;
  align-items: center;
}

.col {
  display: flex;
  flex-direction: column;
}
</style>
