<template>
  <div class="about_me">
    <span class="iconfont icon-ditu2"></span>自我介绍
    <div class="about-me__content">
      <div>3年前端经验</div>
      <div>熟练使用Angular/react/vue/jquery 开发页面</div>
      <div>拥有ionic webApp、 Flutter 开发android/ios app 经验</div>
      <div>熟悉 websocket/http 的使用</div>
      <div>拥有一定的运维基础，会基础的管理服务器站点</div>
      <div>将前端项目打包进 Docker 运行</div>
    </div>
  </div>
</template>
<!-- Add "scoped" attribute to limit CSS to this component only -->
<style scoped>
.about_me div {
  margin-bottom: 2px;
}
.about_me {
  background: #fff;
  border-radius: 18px;
  width: 341px;
  text-align: left;
  padding: 20px 32px;
  font-family: cursive;
}

.right .about-me__content {
  margin-top: 10px;
  font-size: 12px;
}

.iconfont {
  font-size: 32px;
}
</style>
