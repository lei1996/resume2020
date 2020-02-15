<template>
  <div class="c-list_container">
    <div class="list">
      <div v-for="(data, index) in datas" :key="index">
        <Company :data="data" />
      </div>
    </div>
  </div>
</template>

<script>
import Company from "./Company.vue";

export default {
  components: {
    Company
  },
  data() {
    return {
      swiperOption: {
        slidesPerView: 2
        // spaceBetween: 30,
      },
      datas: [
        {
          name: "金鼎园",
          money: "23k",
          time: "2018/09-2019/12",
          category: "互联网/电子商务",
          details: "负责web前端开发。与后端美工产品共同协同完成项目。"
          //   link: "https://github.com/lei1996/fiora-app-flutter"
        },
        {
          name: "长沙依磁网络科技有限公司",
          money: "8k",
          time: "2018/02-2018/07",
          category: "互联网/电子商务",
          details: "负责web前端开发。与后端美工产品共同协同完成项目。"
          //   link: "https://github.com/lei1996/fiora-app-flutter"
        },
        {
          name: "湖南无为网电子商务有限公司",
          money: "6k",
          time: "2017/08-2018/01",
          category: "互联网/电子商务",
          details:
            "为企业定制开发后台管理系统，维护之前的老系统。使用第三方UI框架 material-ui 和 element-ui 完成业务."
          //   link: "https://github.com/lei1996/fiora-app-flutter"
        },
        {
          name: "湖南福米云信息科技有限公司",
          money: "4k",
          time: "2016/06-2016/11",
          category: "互联网/电子商务",
          details: "路由器控制台页面 用h5+css+js重写路由器页面。"
          //   link: "https://github.com/lei1996/fiora-app-flutter"
        }
      ]
    };
  }
};
</script>

<!-- Add "scoped" attribute to limit CSS to this component only -->
<style scoped>
.c-list_container {
  margin-top: 27px;
}
.list {
  /* display: flex; */
  /* width: 720px; */
}

.p-list_container {
  margin-top: 27px;
}
</style>
