<template>
  <div id="app">
    <header>
    <!-- router-link 定义点击后导航到哪个路径下 -->
      <router-link to="/">Home</router-link>
      <router-link to="/about">About</router-link>
    </header>
    <!-- 对应的组件内容渲染到router-view中 -->
    <router-view></router-view> 
  </div>
</template>

<script>
import Hello from './components/Hello.vue'
import About from './components/About.vue'
export default {
  name: 'app',
  components: {
    Hello,
    About
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
a{
  margin:0 10px
}
</style>
