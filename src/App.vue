<template>
  <div id="app">
    <Button :disabled=false @onceClick="AppClick">提交按钮</Button>
  </div>
</template>

<script>
import Button from './components/Button.vue'
export default {
  name: 'App',
  components: {
    Button
  },
  methods: {
    AppClick(){
      alert("你点击了我!");
    }
  },
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
