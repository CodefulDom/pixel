<template>
  <div class="canvas">
    <Pixel v-for="n in 900" color="blue" :key="n" />
  </div>
</template>

<script>
import Pixel from './Pixel'

export default {
  name: 'App',
  components: {
    Pixel
  }
}
</script>
<style scoped>
.canvas {
  display: flex;
  flex-wrap: wrap;
  max-width: 900px;
}
</style>
