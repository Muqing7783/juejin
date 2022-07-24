<template>
  <el-tabs v-model="activeName" @tab-click="handleClick">

    <el-tab-pane label="综合" name="first">综合</el-tab-pane>
    <el-tab-pane label="关注" name="second">关注</el-tab-pane>
    <el-tab-pane label="后端" name="third">后端</el-tab-pane>
    <el-tab-pane label="Android" name="fourth">Android</el-tab-pane>
    <el-tab-pane label="iOS" name="fifth">iOS</el-tab-pane>
    <el-tab-pane label="人工智能" name="sixth">人工智能</el-tab-pane>
    <el-tab-pane label="开发工具" name="seventh">开发工具</el-tab-pane>
    <el-tab-pane label="代码人生" name="eighth">代码人生</el-tab-pane>
    <el-tab-pane label="阅读" name="ninth">阅读</el-tab-pane>
  </el-tabs>
</template>

<script>
export default {
  data() {
    return {
      activeName: 'first'
    };
  },
  methods: {
    handleClick(tab, event) {
      console.log(tab, event);
    }
  }
};
</script>

<style scoped>

</style>
