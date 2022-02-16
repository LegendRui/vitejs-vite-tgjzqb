<template>
  <div class="common-layout">
    <el-container>
      <el-header>
        <CustomHeader />
      </el-header>
      <el-container>
        <el-aside width="200px"> <CustomAside /></el-aside>
        <el-container>
          <el-main>Main</el-main>
        </el-container>
      </el-container>
    </el-container>
  </div>
</template>

<script lang="ts" setup>
import CustomHeader from './CustomHeader.vue';
import CustomAside from './CustomAside.vue';
</script>

<style scoped>
.common-layout .el-header,
.common-layout .el-footer {
  background-color: skyblue;
  color: var(--el-text-color-primary);
  text-align: center;
  height: 60px;
  padding: 0 !important;
  margin: 0 !important;
}
.common-layout .el-footer {
  line-height: 60px;
}

.common-layout .el-aside {
  background-color: #d3dce6;
  color: var(--el-text-color-primary);
  text-align: center;
  position: fixed;
  top: 60px;
  height: calc(100% - 60px);
}

.common-layout .el-main {
  background-color: #e9eef3;
  color: var(--el-text-color-primary);
  text-align: center;
  position: fixed;
  top: 60px;
  left: 200px;
  width: calc(100% - 200px);
  height: calc(100% - 60px);
}

.common-layout > .el-container {
  margin-bottom: 40px;
}

.common-layout .el-container:nth-child(5) .el-aside,
.common-layout .el-container:nth-child(6) .el-aside {
  line-height: 260px;
}

.common-layout .el-container:nth-child(7) .el-aside {
  line-height: 320px;
}
</style>
