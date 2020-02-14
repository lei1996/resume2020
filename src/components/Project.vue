<template>
  <div class="project">
    <div class="backimg"></div>
    <div class="flex-box">
      <div class="name">{{ data.name }}</div>
      <div class="time">{{ data.time }}</div>
    </div>
    <div class="detail">
      {{ data.detail }}
    </div>
    <div class="detail xiangxi">
      {{ data.xiangxi }}
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
.project {
  color: #fff;
  background: #3f4546;
  border-radius: 18px;
  padding: 36px 32px;
  /* width: 289px; */
  text-align: left;
  font-size: 11px;
  font-family: cursive;
  height: 100%;
  position: relative;
  overflow: hidden;
  /* background-position: 32% 19%; */
}
.backimg {
  background: url("https://i.picsum.photos/id/377/322/170.jpg") no-repeat;
  filter: blur(4px);
  position: absolute;
  top: 0;
  left: 0;
  width: 100%;
  height: 100%;
}
.project:first-child {
  margin: 0 19px;
}

.flex-box {
  display: flex;
  justify-content: space-between;
  align-items: center;
}

.name {
  font-size: 14px;
  z-index: 22;
}

.time {
  transform: scale(0.75);
  transform-origin: center right;
}

.detail {
  margin-top: 8px;
  transform: scale(0.9);
  font-family: auto;
  width: 113%;
  transform-origin: left top;
}

.xiangxi {
  margin-top: 2px;
}

.iconfont {
  font-size: 32px;
}
</style>
