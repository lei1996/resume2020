<template>
  <div class="project">
    <span class="iconfont icon-xiangmu"></span> 项目
    <div class="container">
      <div class="flex-box">
        <div class="name">开心聊网页</div>
        <div class="time">2018/09-2018/12</div>
      </div>
      <div class="detail">
        React+mobx 构建的一个能够实时聊天的单页面SPA站点。
      </div>
      <div class="detail xiangxi">
        负责项目主要开发工作。（项目构建到页面实现到对接接口到连接sdk收发消息，最后打包测试生产发布。）
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
<!-- Add "scoped" attribute to limit CSS to this component only -->
<style scoped>
.project {
  color: #fff;
  border-radius: 18px;
  width: 289px;
  text-align: left;
  margin-left: 19px;
  padding: 20px 32px;
  font-size: 11px;
  font-family: cursive;
}

.container {
  background: #3f4546;
  border-radius: 18px;
  padding: 20px 32px;
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
