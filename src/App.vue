<template>
  <div id="app">
    <p>移动端图片上传预览组件：</p>
    <Upload max="3" @listenToUpload="receiveUpload"/>
  </div>
</template>

<script>
import Upload from './components/Upload'

export default {
  name: 'App',
  components: {
    Upload
  },
  methods:{
    receiveUpload (data) {
      console.log(data)
    }
  }
}
</script>

<style>
#app {
  font-family: 'Avenir', Helvetica, Arial, sans-serif;
  -webkit-font-smoothing: antialiased;
  -moz-osx-font-smoothing: grayscale;
  text-align: center;
  color: #2c3e50;
  margin-top: 60px;
}
</style>
