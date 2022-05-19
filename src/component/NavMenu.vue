<template>
  <el-menu :default-active="activeIndex" class="el-menu-demo" mode="horizontal" @select="handleSelect">
    <el-menu-item index="1">首页</el-menu-item>
    <!-- <el-submenu index="2">
      <template slot="title">我的工作台</template>
      <el-menu-item index="2-1">选项1</el-menu-item>
      <el-menu-item index="2-2">选项2</el-menu-item>
      <el-menu-item index="2-3">选项3</el-menu-item>
      <el-submenu index="2-4">
        <template slot="title">选项4</template>
        <el-menu-item index="2-4-1">选项1</el-menu-item>
        <el-menu-item index="2-4-2">选项2</el-menu-item>
        <el-menu-item index="2-4-3">选项3</el-menu-item>
      </el-submenu>
    </el-submenu> -->
    <!-- <el-menu-item index="3" disabled>消息中心</el-menu-item> -->
    <!-- <el-menu-item index="4"><a href="https://www.ele.me" target="_blank">订单管理</a></el-menu-item> -->
    <el-menu-item index="2">华语</el-menu-item>
    <el-menu-item index="3">欧美</el-menu-item>
    <el-menu-item index="4">日韩</el-menu-item>
    <el-menu-item index="5">流行</el-menu-item>
    <el-menu-item index="6">摇滚</el-menu-item>
    <el-menu-item index="7">民谣</el-menu-item>
    <el-menu-item index="8">电子</el-menu-item>
    <el-menu-item index="9">轻音乐</el-menu-item>
    <el-menu-item index="10">影视原声音</el-menu-item>
    <el-menu-item index="11">ACG</el-menu-item>
    <el-menu-item index="12">另类/独立</el-menu-item>
    <li role="menuitem" tabindex="0" class="el-menu-item" style="border-bottom-color: transparent;">
      <global-search></global-search>
    </li>

    <li id="login_link" role="menuitem" tabindex="0" class="el-menu-item" style="border-bottom-color: transparent;">
      <el-link icon="el-icon-user" href="https://www.baidu.com" target="_blank">登录</el-link>
    </li>
  </el-menu>
</template>
<script>
import GlobalSearch from './GlobalSearch.vue'
export default {
  components: {
    GlobalSearch
  },
  data() {
    return {
      activeIndex: '1'
    };
  },
  methods: {
    handleSelect(key, keyPath) {
      console.log(key, keyPath);
    }
  }
}
</script>
<style>
#login_link {
  float: right;
}
</style>