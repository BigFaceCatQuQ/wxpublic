<template>
  <div class="introduce">
      <div class="companyIntroduce"></div>
      <div class="aboutCompany">
          <div style="height:35px;font-size:24px;">
              我们的服务
          </div>
          <div style="height:30px;color:grey">
              our services
          </div>
          <div>
              <img src="../assets/circle.png" alt="">
          </div>
          <div style="font-size:24px;color:red;padding:10px 0">
              远程协助 + 远程会议 + 远程监督 + 实时对讲 = <span style="font-size:36px;color:black;font-weight:600;border-bottom:5px solid #959595">远 信</span>
          </div>
          <div style="padding:5px 20%">
              上海见慧企业发展有限公司成立于2016年5月，致力于生产过程智能化和生产管理互联网化的研究和市场发展工作。2018年7月，公司研究团队瞄准单人分散作业相关行业存在的管理难题，开展了大量研究和产品开发工作，打造了工业互联网概念产品“远信”。
          </div>
      </div>
  </div>
</template>

<script>
export default {
  name: "Introduce",
  data() {
    return {
    };
  },
  methods: {},
  mounted() {

  }
};
</script>

<style scoped>
.introduce {
    width: 100%;
    height: 100%;
}
.companyIntroduce {

}
.aboutCompany {
    width:100%;
    height: 70%;
}
</style>