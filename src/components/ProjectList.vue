<template>
  <div class="p-list_container">
    <!-- <span class="iconfont icon-xiangmu"></span> 项目 -->
    <div class="list">
      <swiper :options="swiperOption" class="swipe">
        <swiper-slide v-for="(data, index) in datas" :key="index">
          <Project :data="data" />
        </swiper-slide>
      </swiper>
    </div>
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
      swiperOption: {
        slidesPerView: 2
        // spaceBetween: 30,
      },
      datas: [
        {
          name: "Flutter IM 在线聊天室APP",
          time: "2020/01-至今",
          detail:
            "使用 Flutter 开发，通讯方式：socket_io_client状态 管理管理：provider",
          xiangxi: "项目地址：https://github.com/lei1996/fiora-app-flutter",
          link: "https://github.com/lei1996/fiora-app-flutter"
        },
        {
          name: "开心聊网页",
          time: "2018/09-2018/12",
          detail: "React+mobx 构建的一个能够实时聊天的单页面SPA站点。",
          xiangxi:
            "负责项目主要开发工作。（项目构建到页面实现到对接接口到连接sdk收发消息，最后打包测试生产发布。）",
          link: "https://www.chatkx.com/"
        },
        {
          name: "虚拟货币量化管理交易平台",
          time: "2018/05-2018/07",
          detail: "使用 angular6 做的一个后台管理项目",
          xiangxi: "负责项目主要开发工作。"
        },
        {
          name: "区块链钱包",
          time: "2018/04-2018/05",
          detail:
            "使用 ionic 3 开发webApp 区块链钱包。 下载地址：https://fir.im/bocaichain",
          xiangxi: "负责项目主要开发工作。",
          link: "https://fir.im/bocaichain"
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
  width: 720px;
}

.p-list_container {
  margin-top: 27px;
}
</style>
