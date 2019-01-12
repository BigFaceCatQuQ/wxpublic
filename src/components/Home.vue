<template>
  <div class="home">
    <el-header>
      <div class="top">
        <el-row>
          <el-col :span="12">
            <div style="blackground-color:red" class="grid-content bg-purple"> <img src="../assets/LOGO.png" /> </div>
          </el-col>
          <el-col :span="12">
            <div style="blackground-color:black" class="grid-content bg-purple-light"></div>
          </el-col>
        </el-row>
      </div>
    </el-header>
    <el-main>
      <div class="centre"></div>
    </el-main>
    <el-footer>
      <div class="bottom"></div>
    </el-footer>
  </div>
</template>

<script>
export default {
  name: "Home"
};
</script>

<style scoped>
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

</style>
