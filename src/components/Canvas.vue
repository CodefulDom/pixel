<template>
  <div class="canvas">
    <Pixel v-for="n in 900" :key="n" color="blue" />
  </div>
</template>
<script>
import Pixel from './Pixel'
export default {
  name: 'Canvas',
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
