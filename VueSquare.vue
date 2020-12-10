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
  position: absolute;
  left: 50%;
  top: 50%;
  margin-top: -200px;
  margin-left: -50px;
  width: 100px;
  height: 100px;
  background: hotpink;
  display: flex;
  font-size: 28px;
  align-items: center;
  justify-content: center;
  border-radius: 50%;
  animation: scale 3s infinite backwards;
}
@keyframes scale {
  100%{
    transform: scale(2);
  }
}
</style>