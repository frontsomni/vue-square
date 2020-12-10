<template>
  <div><span :style="{
    color: textColor
  }">{{text}}</span></div>
</template>

<script>
export default {
  name: 'VueSquare',
  props: {
    text: {
      type: String,
      default: 'vue-square'
    },
    textColor: {
      type: String,
      default: '#fff'
    }
  }
}
</script>

<style scoped>
div{
  width: 100px;
  height: 100px;
  background: #c20;
}
</style>