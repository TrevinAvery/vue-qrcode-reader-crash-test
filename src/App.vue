<template>
  <div id="app">
    <QrcodeReader/>
  </div>
</template>

<script>
import QrcodeReader from './components/QrcodeReader.vue'

export default {
  name: 'App',
  components: {
    QrcodeReader
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
