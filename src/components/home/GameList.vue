<template>
  <div>
    <el-tabs>
      <el-tab-pane>
        <span slot="label"
              class="toplist">精品推荐</span>
        <ul class='gameList'>
          <li v-for="item in images"
              :key="item.url">
            <span class="gameImg"><img :src="item.url"
                   width=100%></span>
            <span class="gemeName">三十六计</span>
          </li>

        </ul>
      </el-tab-pane>

      <el-tab-pane label="敬请期待">
        <span>404-error!!!</span>
      </el-tab-pane>
    </el-tabs>

  </div>
</template>

<script>
export default {
  data () {
    return {
      images: [
        { url: require("../../assets/game_img/img1.jpg") },
        { url: require("../../assets/game_img/img2.jpg") },
        { url: require("../../assets/game_img/img3.jpg") },
        { url: require("../../assets/game_img/img4.jpg") },
        { url: require("../../assets/game_img/img5.jpg") },
        { url: require("../../assets/game_img/img6.jpg") },
      ]
    }
  },
}
</script>

<style scoped>
.gemeList ul,
li {
  list-style: none;
  width: 30%;
  border: 1px solid #e5e9f2;
  height: auto;
  overflow: hidden;
  background-color: #fff;
  padding: 2px;
  float: left;
  margin: 2px;
  font-size: 16px;
  color: brown;
}
.toplist {
  color: red;
}
</style>