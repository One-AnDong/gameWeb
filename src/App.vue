<template>
  <div id="app">
    <div class="header">
      <headlist></headlist>
    </div>

    <div class="router">
      <router-view></router-view>
    </div>

    <div class="tips">
      <tips></tips>
    </div>
    <div class="foot">
      <foot></foot>
    </div>

  </div>
</template>

<script>
import tips from "@/components/Tips"
import foot from "@/components/Foot"
import headlist from '@/components/Header'
export default {
  name: 'App',
  components: {
    foot,
    tips,
    headlist
  },
  // mounted() {
  //   document.querySelector('#audio').play()
  // }
}
</script>

<style lang="less">
@import 'assets/styles/index.less';
#app {
  font-family: '微软雅黑', Helvetica, Arial, sans-serif;
  -webkit-font-smoothing: antialiased;
  -moz-osx-font-smoothing: grayscale;
  text-align: center;
  color: #2c3e50;
  width: 1200px;
  margin: 0 auto;
  background-color: #f1f4f9;
}
.header {
  border-top: 1px solid #d2d5da;
  background-color: white;
}
.foot {
  background: #fff;
}
.tips {
  float: none;
}

.router {
  margin: 0 auto;
}
</style>
