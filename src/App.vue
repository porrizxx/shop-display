<template>
  <el-container>
    <el-header>
      <page-head></page-head>
    </el-header>
    <el-header>
      <nav-bar></nav-bar>
    </el-header>
    <el-main><router-view /></el-main>
    <el-footer>Footer</el-footer>
  </el-container>
</template>

<script>
import NavBar from "./components/common/NavBar";
import PageHead from "./components/common/PageHead";

export default {
  name: "Home",
  components: {
    NavBar,
    PageHead
  }
};
</script>

<style>
.el-header,
.el-footer {
  /* background-color: #b3c0d1; */
  color: #333;
  text-align: center;
  line-height: 60px;
}

.el-aside {
  background-color: #d3dce6;
  color: #333;
  text-align: center;
  line-height: 200px;
}

.el-main {
  background-color: #e9eef3;
  color: #333;
  text-align: center;
  line-height: 160px;
}

body > .el-container {
  margin-bottom: 40px;
}

.el-container:nth-child(5) .el-aside,
.el-container:nth-child(6) .el-aside {
  line-height: 260px;
}

.el-container:nth-child(7) .el-aside {
  line-height: 320px;
}
</style>
