<template>
  <div class="project">
    <span class="iconfont icon-xiangmu"></span> 项目
    <Project />
  </div>
</template>

<script>
import Project from "./Project.vue";

export default {
  components: {
    Project
  },
  data() {
    return {
      barWidth: "50"
    };
  }
};
</script>

<!-- Add "scoped" attribute to limit CSS to this component only -->
<style scoped>
</style>
