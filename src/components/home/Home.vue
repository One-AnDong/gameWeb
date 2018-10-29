<template>
  <div class="home">
    <el-row>
      <div>
        <el-col :span="24">
          <carousel></carousel>
        </el-col>
      </div>

    </el-row>

    <el-row class="main">
      <el-col :span="18">
        <div>
          <gamelist height="654px"></gamelist>
        </div>
      </el-col>

      <el-col :span="6">
        <div class="login">
          <login></login>
        </div>
      </el-col>
    </el-row>

    <el-row>
      <div class="extend">
        <el-col :span="6">
          <div class="extend-content">海外平台</div>
        </el-col>
        <el-col :span="6">
          <div class="extend-content">客户服务</div>
        </el-col>
        <el-col :span="6">
          <div class="extend-content">游戏美女</div>
        </el-col>
        <el-col :span="6">
          <div class="extend-content">
            <router-link to="/guardian"
                         target="_blank">未成年人监护</router-link>
          </div>
        </el-col>
      </div>
    </el-row>
    <div>
      <cover-layer></cover-layer>
    </div>
  </div>
</template>

<script>  
import coverLayer from '@/components/CoverLayer'
import gamelist from '@/components/home/Recommend'
import carousel from '@/components/home/Carousel'
import login from '@/components/Login'
export default {
  name: 'home',
  components: {
    gamelist,
    carousel,
    login,
    coverLayer
  }
}
</script>

<style scoped>
.main {
  padding-top: 20px;
  background-color: #fff;
}
.extend {
  height: 40px;
  margin-top: 30px;
  margin-bottom: 70px;
}
.extend-content {
  background: #fff;
  padding: 15px 10px;
  margin: 0 20px;
  border-radius: 10px;
  height: 40px;
  line-height: 40px;
  text-align: center;
}
.login {
  margin-left: 10px;
}
</style>