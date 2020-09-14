<template>
  <h2>{{ content }}</h2>
</template>

<script>
export default {
  props: ["content"]
}
</script>

<style lang="scss" scoped>
h2{
  font-size: 18px;
  font-weight: bold;
  text-align: center;
  margin-bottom: 1em;
  position: relative;
  &::before{
    content: '';
    position: absolute;
    bottom: -15px;
    display: inline-block;
    width: 60px;
    height: 5px;
    left: 50%;
    transform: translateX(-50%);
    background-color: black;
    border-radius: 2px;
  }
}
</style>