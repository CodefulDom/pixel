<template>
  <div :class="['pixel', color]"></div>
</template>

<script>
export default {
  name: 'Pixel',
  props: {
    color: String
  }
}
</script>
<style lang="scss">
.pixel {
  border: 1px solid lightgrey;
  width: 30px;
  height: 30px;
  box-sizing: border-box;
}
.white {
  background-color: white;
}

.lightBlue {
  background-color: rgb(0, 188, 212);
}

.blue {
  background-color: rgb(3, 169, 244);
}

.darkBlue {
  background-color: rgb(33, 150, 243);
}
</style>
