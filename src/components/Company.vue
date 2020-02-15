<template>
  <div class="company">
    <div class="company_box">
      <div class="company_flexbox">
        <div class="name">金鼎园</div>
        <div class="money">23k</div>
      </div>
      <div class="time">2018/09-2019/12</div>
      <div class="category">互联网/电子商务</div>
      <div class="details">
        负责web前端开发。与后端美工产品共同协同完成项目。
      </div>
    </div>
  </div>
</template>

<script>
// import Project from "./Project.vue";

export default {
  components: {
    // Project
  },
  data() {
    return {
      //   swiperOption: {
      //     slidesPerView: 2
      //     // spaceBetween: 30,
      //   },
    };
  }
};
</script>

<!-- Add "scoped" attribute to limit CSS to this component only -->
<style scoped>
@import url("https://fonts.googleapis.com/css?family=Noto+Sans+SC&display=swap");

.company {
  display: flex;
  width: 720px;
  margin-top: 20px;
}
.company .company_box {
  background: #272b2f;
  color: #fff;
  padding: 37px 20px;
  margin: 0 19px;
  border-radius: 16px;
  text-align: left;
}
.company .name {
  font-weight: bold;
  font-size: 20px;
  font-family: "Noto Sans SC", sans-serif;
}
.company .category {
  font-size: 13px;
  margin-top: 8px;
  color: #f9403c;
}
.company .details {
  font-size: 12px;
  color: #febc2f;
  margin-top: 2px;
}
.company .money {
  background: #febc2c;
  border-radius: 50%;
  height: 40px;
  width: 40px;
  font-size: 11px;
  color: #403b2d;
  font-weight: bold;
  text-align: center;
  line-height: 40px;
}
.company .company_flexbox {
  display: flex;
  justify-content: space-between;
  align-items: center;
}
.company .time {
  color: #999a9b;
  font-size: 11px;
  font-family: monospace;
}
</style>
