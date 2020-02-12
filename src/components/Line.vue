<template>
  <div class="bar">
    <div :style="{ width: width + 'px' }" class="bar-line"></div>
  </div>
</template>

<script>
export default {
  props: {
    barWidth: String
  },
  data() {
    return {
      width: '0'
    };
  },
  mounted() {
    this.width = this.barWidth;
  }
};
</script>

<!-- Add "scoped" attribute to limit CSS to this component only -->
<style scoped>
.bar {
  width: 100px;
  height: 10px;
  background: #fff;
  border-radius: 2px;
  overflow: hidden;
}

.bar .bar-line {
  width: 0px;
  height: 10px;
  background: rgba(179, 181, 198, 1);
  border-radius: 2px;
  transition: all 0.55s ease-out;
}
</style>
