<template>
  <div id="app">
    <el-row>
      <el-col>
        <div class="grid-content bg-purple">
          <el-menu class="el-menu-demo" mode="horizontal">
            <el-menu-item index="1">互联网</el-menu-item>
            <el-menu-item index="2">法律</el-menu-item>
            <el-menu-item index="3">金融</el-menu-item>
          </el-menu>
        </div>
      </el-col>
    </el-row>
    <el-row>
      <el-col>
        <div class="grid-content bg-purple">
          <router-view></router-view>
        </div>
      </el-col>
    </el-row>
  </div>
</template>

<script>
export default {
  name: 'app',
};
</script>

<style>
body {
  margin: 0;
  min-width: 1200px;
}
</style>
