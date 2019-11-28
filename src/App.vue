<template>
  <div id="app">
    <ColorPicker :color="color" />
    <Canvas />
  </div>
</template>

<script>
import Canvas from './components/Canvas'
import ColorPicker from './components/ColorPicker'

export default {
  name: 'App',
  components: {
    Canvas,
    ColorPicker
  },
  data() {
    return {
      color: 'white'
    }
  },
  mounted() {
    this.$root.$on('updatecolor', (color) => {
      this.color = color
    })
  }
}
</script>

<style>
#app {
  font: 'Avenir', Helvetica, Arial, sans-serif;
  -webkit-font-smoothing: antialiased;
  -moz-osx-font-smoothing: grayscale;
  text-align: center;
  color: #2c3e50;
  margin-top: 60px;
  background-color: #333;
  display: flex;
  align-items: center;
  height: 100px;
}
</style>
