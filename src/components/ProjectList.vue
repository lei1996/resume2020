<template>
  <div class="project">
    <span class="iconfont icon-xiangmu"></span> 项目
    <div class="list">
      <div v-for="(data, index) in datas" :key="index">
        <Project :data="data" />
      </div>
    </div>
    <!-- <div>
      <div>2018/05-2018/07 虚拟货币量化管理交易平台</div>
      <div>使用 angular6 做的一个后台管理项目</div>
      <div>
        负责项目主要开发工作。
      </div>
    </div>
    <div>
      <div>2018/04-2018/05 区块链钱包</div>
      <div>
        使用 ionic 3 开发webApp 区块链钱包。 下载地址，https://fir.im/bocaichain
      </div>
      <div>
        负责项目主要开发工作。
      </div>
    </div> -->
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
      datas: [
        {
          name: "开心聊网页",
          time: "2018/09-2018/12",
          detail: "React+mobx 构建的一个能够实时聊天的单页面SPA站点。",
          xiangxi:
            "负责项目主要开发工作。（项目构建到页面实现到对接接口到连接sdk收发消息，最后打包测试生产发布。）"
        },
        {
          name: "开心聊网页",
          time: "2018/09-2018/12",
          detail: "React+mobx 构建的一个能够实时聊天的单页面SPA站点。",
          xiangxi:
            "负责项目主要开发工作。（项目构建到页面实现到对接接口到连接sdk收发消息，最后打包测试生产发布。）"
        }
      ]
    };
  }
};
</script>

<!-- Add "scoped" attribute to limit CSS to this component only -->
<style scoped>
.list {
  display: flex;
}
</style>
