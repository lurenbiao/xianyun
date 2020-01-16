<template>
  <div class="header-wrapper">
    <el-row type="flex" justify="space-between" align="middle" class="header">
      <!-- logo -->
      <div class="logo">
        <nuxt-link to="/">
          <img src="/logo.jpg" alt />
        </nuxt-link>
      </div>

      <!-- 菜单栏 -->
      <el-row type="flex" class="navs">
        <nuxt-link to="/">首页</nuxt-link>
        <nuxt-link to="/post">旅游攻略</nuxt-link>
        <nuxt-link to="/hotel">酒店</nuxt-link>
        <nuxt-link to="/air">国内机票</nuxt-link>
      </el-row>

      <div class="user">
        <nuxt-link to="/user">登录/注册</nuxt-link>
      </div>
    </el-row>
  </div>
</template>

<script>
export default {};
</script>

<style lang='less' scoped>
.header-wrapper {
  min-width: 1000px;
  background-color: #fff;
  border-bottom: 1px solid #eee;
  box-shadow: 0px 3px 4px #f6f6f6;
  position: relative;
  z-index: 2;
  height: 60px;
}
.header {
  width: 1000px;
  margin: 0 auto;
  height: 60px;
  .logo {
    img {
      width: 156px;
      height: 42px;
      display: block;
    }
  }
  .navs {
    flex: 1;
    margin-left: 20px;

    a {
      display: block;
      height: 60px;
      padding: 0px 20px;
      box-sizing: border-box;
      line-height: 60px;
      &:hover {
        border-bottom: 2px solid skyblue;
        color: skyblue;
      }
    }
  }
}
.user{
    font-size: 14px;
    color: #053744
}
</style>