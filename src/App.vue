<template>
  <div id="app">
    <van-tabbar v-model="active" route="">
      <van-tabbar-item replace icon="home-o" to="/">首页</van-tabbar-item>
      <van-tabbar-item replace icon="search" to="/about">课程</van-tabbar-item>
      <van-tabbar-item replace icon="friends-o">约课记录</van-tabbar-item>
      <van-tabbar-item replace icon="setting-o">练习</van-tabbar-item>
      <van-tabbar-item replace icon="setting-o">我的</van-tabbar-item>
    </van-tabbar>
    <router-view />
  </div>
</template>

<script>
export default {
  data () {
    return {
      active: 0
    }
  }
}
</script>

<style lang="scss">
* {
  padding: 0;
  margin: 0;
}
</style>
