<template>
  <div class="custom-header">
    <div class="avatar">
      <el-dropdown>
        <el-avatar :size="30" :src="circleUrl"></el-avatar>
        <template #dropdown>
          <el-dropdown-menu>
            <el-dropdown-item>用户中心</el-dropdown-item>
            <el-dropdown-item>Action 2</el-dropdown-item>
          </el-dropdown-menu>
        </template>
      </el-dropdown>
    </div>
  </div>
</template>
<script lang="ts" setup>
const circleUrl =
  'https://cube.elemecdn.com/3/7c/3ea6beec64369c2642b92c6726f1epng.png';
</script>
<style lang="less" scoped>
.custom-header {
  display: flex;
  height: 60px;
  justify-content: flex-end !important;
  align-content: center;
  align-items: center;
}
.avatar {
  margin-right: 12px;
}
</style>
