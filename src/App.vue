<template>
  <div id="app">
    <img alt="Vue logo" src="./assets/logo.png">
    <HelloWorld :msg="msg" :content="content" :flag="flag" :res="res"/>
    <p>
      <input type="text" v-model="res">
    </p>
    <button @click="alerts">点击弹框</button>
    卧槽
  </div>
</template>

<script>
import HelloWorld from './components/HelloWorld.vue'

export default {
  name: 'App',
  data(){
    return{
      msg:"小姐姐 真好看",
      flag:false,
      res:"",
      content:"卧槽 我还是个孩子啊 就这样对我？？？"
    }
  },
  components: {
    HelloWorld
  },
  methods:{
    alerts(){
       this.flag=!this.flag;
    }
  }
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
