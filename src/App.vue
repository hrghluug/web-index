<template>
  <div id="app">
    <el-container>
      <el-header>
        <el-row :gutter="20" class="inherit-height">
          <el-col :span="8" class="inherit-height">
            <HeaderLeft />
          </el-col>
          <el-col :span="8" class="inherit-height">
            <HeaderCenter />
          </el-col>
          <el-col :span="8" class="inherit-height">
            <HeaderRight />
          </el-col>
        </el-row>
      </el-header>
      <el-main>Main</el-main>
    </el-container>
  </div>
</template>
<script>
// @ is an alias to /src
import HeaderLeft from "@/components/header/HeaderLeft";
import HeaderCenter from "@/components/header/HeaderCenter";
import HeaderRight from "@/components/header/HeaderRight";

export default {
  name: "app",
  components: {
    HeaderLeft,
    HeaderCenter,
    HeaderRight
  }
};
</script>
<style lang="scss">
#app {
  font-family: Avenir, Helvetica, Arial, sans-serif;
  -webkit-font-smoothing: antialiased;
  -moz-osx-font-smoothing: grayscale;
  text-align: center;
  color: #2c3e50;


}
.inherit-height {
  height: inherit;
}
nav {
  padding: 30px;

  a {
    font-weight: bold;
    color: #2c3e51;

    &.router-link-exact-active {
      color: #42b983;
    }
  }
}
</style>
