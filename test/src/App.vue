<template>
  <div id="app">
    <el-container>
      <el-header>
        <h1>美食功能列表</h1>
      </el-header>
      <el-container>
        <el-aside-col>
          <el-menu :default-openeds="['1']" style=" background: #93F393;">
            <el-submenu router index="1">
                <template slot="title">
                  北方美食
                  <router-link>北方美食</router-link>
                </template>
            </el-submenu>
            <el-submenu index="/hi" router >
                <template slot="title">
                  <router-link>发布美食</router-link>
                </template>
            </el-submenu>
          </el-menu>
        </el-aside-col>
        <el-main>
          <router-view></router-view>
        </el-main>
      </el-container>
    </el-container>
  </div>
</template>

<script>
export default {
  name: 'App'
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
