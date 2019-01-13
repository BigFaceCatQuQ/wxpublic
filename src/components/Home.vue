<template>
  <div class="home">
    <el-header height="120px">
      <div class="top">
        <div class="head-left">
          <div class="logo-img">
            <img src="../assets/logo1.png" alt height="120px">
          </div>
          <div class="word">
            <div style="padding:30px 0 0 0;text-align:left">遥可及 远可信</div>
            <div style="padding:10px 0 0 0;text-align:left">远信——实现作业管理的远程化、透明化</div>
          </div>
        </div>
        <div class="head-right">
          <!-- <div class="tag">
            首页
          </div>
          <div class="tag">
            代理招商说明
          </div>
          <div class="tag">
            代理合同文本
          </div>-->
          <el-menu
            class="el-menu-demo"
            mode="horizontal"
          >
            <el-menu-item index="1">首页</el-menu-item>
            <el-menu-item index="2">代理招商说明</el-menu-item>
            <el-menu-item index="3">代理合同文本</el-menu-item>
          </el-menu>
        </div>
      </div>
    </el-header>
    <el-main>
      <div class="centre">
        <el-carousel arrow="always" trigger="click" height="550px">
          <el-carousel-item v-for="item in imgList" :key="item.id">
            <el-col :span="24">
              <img :src="item.idView" width="100%">
            </el-col>
          </el-carousel-item>
        </el-carousel>
      </div>
    </el-main>
    <el-footer>
      <div class="bottom"></div>
    </el-footer>
  </div>
</template>

<script>
export default {
  name: "Home",
  data() {
    return {
      imgList: [
        { id: 0, idView: require("../assets/lunbo1.png") },
        { id: 1, idView: require("../assets/lunbo2.png") }
      ]
    };
  }
};
</script>

<style scoped>
@import url("//unpkg.com/element-ui@2.4.11/lib/theme-chalk/index.css");
.home {
  width: 100%;
  height: 100%;
}

.top {
  width: 100%;
  height: 120px;
  background-color: #ffffff;
}

.centre {
  width: 100%;
  height: 550px;
  background-color: #e8e8e8;
}

.bottom {
  width: 100%;
  height: 550px;
  background-color: #1f2025;
}

.head-left {
  float: left;
  padding-left: 80px;
  width: 50%;
  height: 120px;
}

.head-right {
  float: right;
  width: 50%;
  height: 120px;
}

.logo-img {
  float: left;
  width: 170px;
}

.word {
  float: left;
  height: 120px;
  font-size: 20px;
}

.tag {
  width: 24%;
  float: left;
  padding-top: 50px;
  font-size: 20px;
}
</style>

<style>
.el-carousel__item h3 {
  color: #475669;
  font-size: 14px;
  opacity: 0.75;
  line-height: 150px;
  margin: 0;
}

.el-carousel__item:nth-child(2n) {
  background-color: #99a9bf;
}

.el-carousel__item:nth-child(2n + 1) {
  background-color: #d3dce6;
}
</style>

