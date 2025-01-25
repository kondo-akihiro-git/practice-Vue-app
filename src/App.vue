<template>
<<<<<<< HEAD
  <img alt="Vue logo" src="./assets/logo.png">
  <HelloWorld msg="Welcome to Your Vue.js App"/>
</template>

<script>
import HelloWorld from './components/HelloWorld.vue'

export default {
  name: 'App',
  components: {
    HelloWorld
  }
}
</script>

<style>
#app {
  font-family: Avenir, Helvetica, Arial, sans-serif;
  -webkit-font-smoothing: antialiased;
  -moz-osx-font-smoothing: grayscale;
  text-align: center;
  color: #2c3e50;
  margin-top: 60px;
}
</style>
=======
  <div id="app">
    <DataDisplay />
  </div>
</template>

<script>
import DataDisplay from './components/DataDisplay.vue';

export default {
  components: {
    DataDisplay
  }
};
</script>
>>>>>>> bdf2449 (ディレクトリ修正)
