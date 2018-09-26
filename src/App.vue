<template>
  <div id="app">
    <el-container>
      <el-header class="header-box">
        <Header />
      </el-header>
      <el-container>
        <el-aside class="xg-menu">
          <Menu></Menu>
        </el-aside>
        <el-main class="main-container">
          <router-view></router-view>
        </el-main>
      </el-container>
    </el-container>

  </div>

</template>

<script>
import HelloWorld from './components/HelloWorld.vue'
import Header from './views/Header.vue'
import Menu from './views/Menu.vue'

export default {
  name: 'app',

  components: {
    HelloWorld,
    Header,
    Menu
  }
}
</script>

<style>
.main-container {
  font-family: "Avenir", Helvetica, Arial, sans-serif;
  -webkit-font-smoothing: antialiased;
  -moz-osx-font-smoothing: grayscale;
  text-align: center;
  color: #2c3e50;
   margin-top: 60px;
}
body{
  margin: 0;
  padding: 0;
}
.header-box{
  background: skyblue;
}
.xg-menu{
  width: 200px;
  min-height: calc(100vh - 60px);
}
</style>
