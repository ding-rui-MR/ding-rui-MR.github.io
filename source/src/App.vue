<template>
  <div id="app">
    <img alt="Vue jyou-logo" src="./assets/jyou-logo.png">
    <HelloWorld msg="Welcome , jyou's first website is building ..."/>
    <el-button @click="startHacking">Start</el-button>
  </div>
</template>

<script>
import HelloWorld from './components/HelloWorld.vue'

export default {
  name: 'App',
  components: {
    HelloWorld
  },
  methods: {
    startHacking () {
      this.$notify({
        title: 'Imported successfully',
        type: 'success',
        message: 'If u can see it , it means element-ui already been imported.',
        duration: 5000
      })
    }
  }
}
</script>

<style lang="less">
#app {
  font-family: Helvetica,  sans-serif;
  -webkit-font-smoothing: antialiased;
  -moz-osx-font-smoothing: grayscale;
  text-align: center;
  color: #2c3e50;
  margin-top: 60px;

}
</style>
