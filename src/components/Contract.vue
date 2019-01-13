<template>
  <div class="contract">
    <el-card class="box-card">
      <div slot="header" class="clearfix">
        <span>远信市场开发代理合同</span>
      </div>
      <div v-for="o in 4" :key="o" class="text item">
        {{'列表内容 ' + o }}
      </div>
    </el-card>

  </div>
</template>

<script>
export default {
  name: "Contract",
  data() {
    return {};
  },
  methods: {},
  mounted() {}
};
</script>

<style scoped>
.contract {
  width: 100%;
  height: 100%;
}

.text {
  font-size: 14px;
}

.item {
  margin-bottom: 18px;
}

.clearfix:before,
.clearfix:after {
  display: table;
  content: "";
}
.clearfix:after {
  clear: both;
}

.box-card {
  width: 80%;
  margin: 0 10%;
}
</style>