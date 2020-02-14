<template>
  <div class="project">
    <div class="flex-box">
      <div class="name">{{data.name}}</div>
      <div class="time">{{data.time}}</div>
    </div>
    <div class="detail">
      {{data.detail}}
    </div>
    <div class="detail xiangxi">
      {{data.xiangxi}}
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
  padding: 20px 32px;
  width: 289px;
  text-align: left;
  margin-left: 19px;
  font-size: 11px;
  font-family: cursive;
  /* height: 100%; */
}

.flex-box {
  display: flex;
  justify-content: space-between;
  align-items: center;
}

.name {
  font-size: 14px;
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
