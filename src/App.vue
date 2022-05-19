<template>
  <div id="app">
    <el-row :gutter="20" style="margin-right: 0">
      <el-col :span="16" :offset="4">
        <nav-menu-vue></nav-menu-vue>
      </el-col>
    </el-row>
    <!-- <el-row :gutter="20" style="margin-right: 0">
      <el-col :span="16" :offset="4">
      <left-menu></left-menu>
      </el-col>
    </el-row> -->

<el-row :gutter="20" style="margin-right: 0">
      <el-col :span="16" :offset="4">
      <type-list-vue></type-list-vue>
      </el-col>
    </el-row>
  </div>
</template>

<script>
import NavMenuVue from './component/NavMenu.vue'
import LeftMenu from './component/LeftMenu.vue'
import TypeListVue from './component/TypeList.vue'

export default {
  components: {
    NavMenuVue,
    LeftMenu,
    TypeListVue
  },
  methods: {
    startHacking() {
      this.$notify({
        title: 'It works!',
        type: 'success',
        message: 'We\'ve laid the ground work for you. It\'s time for you to build something epic!',
        duration: 5000
      })
    }
  }
}
</script>

<style>
#app {
  font-family: Helvetica, sans-serif;
  text-align: center;
}

.el-row {
  margin-bottom: 20px;

  &:last-child {
    margin-bottom: 0;
  }
}

.el-col {
  border-radius: 4px;
}

.bg-purple-dark {
  background: #99a9bf;
}

.bg-purple {
  background: #d3dce6;
}

.bg-purple-light {
  background: #e5e9f2;
}

.grid-content {
  border-radius: 4px;
  min-height: 36px;
}

.row-bg {
  padding: 10px 0;
  background-color: #f9fafc;
}
</style>
