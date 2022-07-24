<template>

  <div>
<!--    <img src="http://imgbed.xiaosezmh.xyz/202207241123642.png" alt="logo">-->
    <el-menu :default-active="activeIndex" class="el-menu-demo" mode="horizontal" @select="handleSelect"
             style="display: flex; justify-content: left; align-content: center;">
      <el-menu-item index="1" class="nav-item">首页</el-menu-item>
      <el-menu-item index="2" class="nav-item">沸点</el-menu-item>
      <el-menu-item index="3" class="nav-item">课程</el-menu-item>
      <el-menu-item index="4" class="nav-item">直播</el-menu-item>
      <el-menu-item index="5" class="nav-item">资讯</el-menu-item>
      <el-menu-item index="6" class="nav-item">活动</el-menu-item>
      <el-submenu index="7" class="nav-item">
        <template slot="title">开放社区</template>
        <el-menu-item index="7-1" class="nav-item">青训营社区</el-menu-item>
      </el-submenu>
      <el-menu-item index="8" class="nav-item">商城</el-menu-item>
      <el-menu-item index="9" class="nav-item">APP</el-menu-item>
      <el-menu-item index="10" class="nav-item">插件</el-menu-item>
      <el-input v-model="input" placeholder="探索稀土掘金" style="display: flex; align-items: center;margin:0 20px; width: 600px">
      </el-input>
      <el-button type="primary" style="height: 90%; margin: auto">创作者中心</el-button>
      <el-menu-item index="11" class="nav-item">会员</el-menu-item>
      <i class="el-icon-message-solid" style="margin: auto; font-size: 30px;color: #8a919f"></i>
      <el-avatar src="https://cube.elemecdn.com/0/88/03b0d39583f48206768a7534e55bcpng.png" style="margin: auto 40px auto 0"></el-avatar>
    </el-menu>
  </div>
</template>

<script>
export default {
  data() {
    return {
      activeIndex: '1',
      activeIndex2: '1',
      input: ''
    };
  },
  methods: {
    handleSelect(key, keyPath) {
      console.log(key, keyPath);
    }
  }
}
</script>
<style scoped>
/*img{

}*/
.nav-item{
  font-size: 20px;
}
</style>
