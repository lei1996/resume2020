<template>
  <div class="company">
    <div class="company_box">
      <div class="company_flexbox">
        <div class="name">{{ data.name }}</div>
        <div class="money">{{ data.money }}</div>
      </div>
      <div class="time">{{ data.time }}</div>
      <div class="category">{{ data.category }}</div>
      <div class="details">
        {{ data.details }}
      </div>
    </div>
  </div>
</template>

<script>
export default {
  props: {
    data: Object
  }
};
</script>

<!-- Add "scoped" attribute to limit CSS to this component only -->
<style scoped>
@import url("https://fonts.googleapis.com/css?family=Noto+Sans+SC&display=swap");

.company {
  display: flex;
  width: 720px;
}
.company .company_box {
  background: #272b2f;
  color: #fff;
  padding: 24px 20px;
  margin: 0 19px;
  /* border-radius: 16px; */
  text-align: left;
  width: 444px;
  border-bottom: 1px solid rgba(255, 255, 255, 0.15);
}
.company .name {
  font-weight: bold;
  font-size: 20px;
  font-family: "Noto Sans SC", sans-serif;
  margin-left: 1px;
  letter-spacing: 4px;
  background: #4e5358;
  border-bottom-left-radius: 7px;
  border-bottom-right-radius: 7px;
  border-top-right-radius: 7px;
  padding: 0 4px;
  padding-left: 9px;
  padding-bottom: 2px;
}
.company .category {
  font-size: 13px;
  margin-top: 8px;
  /* color: #f9403c; */
}
.company .details {
  font-size: 12px;
  /* color: #febc2f; */
  margin-top: 2px;
  max-width: 300px;
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
