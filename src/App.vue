<template>
  <!-- <img alt="Vue logo" src="./assets/logo.png"> -->
  <!-- <HelloWorld msg="Welcome to Your Vue.js App"/> -->
  <p :style="{color: color}">Hi</p>
  <Block :color="color"/>
  <Input :colorChanged="updateColor"/>
</template>

<script>
// import HelloWorld from './components/HelloWorld.vue'
import Block from './components/Block.vue'
import Input from './components/Input.vue'

export default {
  name: 'App',
  components: {
    // HelloWorld
    Block,
    Input
  },
  data() {
      return {
        color: 'red'
      }
  },
  methods: {
    updateColor(val) {
      this.color = val
      console.log(this.color)
    }
  },
}
</script>

<style>
/* #app {
  font-family: Avenir, Helvetica, Arial, sans-serif;
  -webkit-font-smoothing: antialiased;
  -moz-osx-font-smoothing: grayscale;
  text-align: center;
  color: #2c3e50;
  margin-top: 60px;
} */
</style>