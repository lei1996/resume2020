<template>
  <div class="container">
    <div class="left">
      <div class="header-portrait">
        <div class="img_box" @click="gotoUrl()">
          <img class="img" src="../assets/logo.png" alt="" />
        </div>
        <div class="color_b"></div>
        <div class="title">
          <div class="name">雷嘉宁</div>
          <div class="occupation">Web front end Engineer</div>
        </div>
      </div>
      <div class="body">
        <div class="contact">
          <div class="phone">
            <span class="iconfont icon-xinbaniconshangchuan-"></span>
            17077460862
          </div>
          <div class="phone">
            <span class="iconfont icon-duanxin"></span> 617218165@qq.com
          </div>
          <div class="phone">
            <span class="iconfont icon-ditu"></span> 湖南 长沙
          </div>
        </div>
      </div>
      <div class="skills">
        <div class="box">
          <RadarComponent
            class="radar"
            :radarData="radarData"
            :options="options"
          />
        </div>
        <div class="btn_box">
          <div class="iconfont__box">
            <span class="iconfont icon-qiehuan"></span>
            <!-- <span class="iconfont icon-iconset0398"></span> -->
          </div>
          <!-- <div><span class="iconfont icon-ditu"></span></div> -->
        </div>
      </div>
    </div>
    <div class="right">
      <AboutMe />
      <ProjectList />
      <CompanyList />
      <!-- 
      <div class="company">
        公司
        <div>
          <div>2018/09-至今 金鼎园</div>
          <div>互联网/电子商务</div>
          <div>23k</div>
          <div>负责web前端开发。与后端美工产品共同协同完成项目。</div>
        </div>
        <div>
          <div>2018/02-07 长沙依磁网络科技有限公司</div>
          <div>互联网/电子商务</div>
          <div>12001-16000元/月</div>
          <div>负责web前端开发。与后端美工产品共同协同完成项目。</div>
        </div>
        <div>
          <div>2017/08-2018/01 湖南无为网电子商务有限公司</div>
          <div>互联网/电子商务</div>
          <div>6001-8000元/月</div>
          <div>为企业定制开发后台管理系统，维护之前的老系统。使用第三方UI框架 material-ui 和 element-ui 完成业务.</div>
        </div>
      </div>
      <div class="education">
        教育
        <div>
          2017/10 - 2020/01 湖南航空工业职工工学院  计算机应用技术   大专
        </div>
        <div>
          2013/09 - 2014/07 五一牛耳学院  电子信息科学与技术   其他
        </div>
        <div>
          2010/09 - 2013/06 长沙市第十九中学  软件   高中
        </div>
      </div> -->
    </div>
  </div>
</template>

<script>
import RadarComponent from "../components/Radar.vue";
import AboutMe from "../components/AboutMe.vue";
import ProjectList from "../components/ProjectList.vue";
import CompanyList from "../components/CompanyList.vue";
// import LineComponent from "../components/Line.vue";

export default {
  components: {
    RadarComponent,
    AboutMe,
    ProjectList,
    CompanyList
    // LineComponent,
  },
  methods: {
    gotoUrl() {
      window.open("https://github.com/lei1996/resume2020");
    }
  },
  data() {
    return {
      barWidth: "50",
      radarData: {
        labels: [
          "Angular",
          "React",
          "Vue.js",
          "linux",
          "Jquery",
          "Flutter",
          "algorithm"
        ],
        datasets: [
          {
            label: "能力值",
            backgroundColor: "rgba(179,181,198,0.2)",
            borderColor: "rgba(179,181,198,1)",
            pointBackgroundColor: "rgba(179,181,198,1)",
            pointBorderColor: "#fff",
            pointHoverBackgroundColor: "#fff",
            pointHoverBorderColor: "rgba(179,181,198,1)",
            data: [75, 83, 73, 45, 68, 77, 27]
          }
        ]
      },
      options: {
        responsive: true,
        maintainAspectRatio: true,
        scale: {
          ticks: {
            beginAtZero: true,
            min: 0
          }
        }
      }
    };
  }
};
</script>

<!-- Add "scoped" attribute to limit CSS to this component only -->
<style scoped>
.container {
  width: 1080px;
  margin: 40px 0;
  /* background: #fff; */
  display: flex;
}

.left {
  flex: 1;
  /* background: red; */
  padding-bottom: 80px;
  background: #fff;
  display: flex;
  justify-content: center;
  align-items: center;
  flex-direction: column;
  position: relative;
  border-right: 1px solid #f8f9fb;
}

.left .img_box:hover {
  box-shadow: 4px 4px 8px rgba(148, 145, 145, 0.6);
}
.left .img_box {
  background: #fff;
  border-radius: 6px;
  width: 150px;
  height: 150px;
  overflow: hidden;
  box-shadow: 4px 4px 8px rgba(148, 145, 145, 0.3);
  transition: all 0.25s ease-out;
  cursor: pointer;
  /* border: 4px solid #545050; */
  position: absolute;
  left: -40px;
  top: -40px;
}

.left .color_b {
  position: absolute;
  top: 0;
  right: 0;
  background: rgba(95, 85, 85, 0.48);
  width: 225px;
  height: 227px;
  border-bottom-left-radius: 57px;
  border-bottom-right-radius: 14px;
}

.left .title {
  margin-top: 145px;
}

.left .name {
  font-size: 26px;
  letter-spacing: 5px;
  font-family: cursive;
}

.left .occupation {
  letter-spacing: 2px;
  font-family: cursive;
  font-style: italic;
}

.left .contact {
  margin-top: 38px;
  display: flex;
  flex-direction: column;
  align-items: start;
}

.left .radar {
  background: #fff;
  width: 200px;
  height: 200px;
}

.left .skills {
  margin-top: 65px;
  padding: 0 42px;
  position: relative;
}

.left .phone {
  font-size: 13px;
  margin-bottom: 5px;
}

.left .phone span {
  margin-right: 10px;
}

.skills .btn_box {
  position: absolute;
  right: 0;
  top: 0;
}
.skills .iconfont__box {
  background: rgba(179, 181, 198, 0.2);
  border-radius: 3px;
  padding: 2px 7px;
  transition: all 0.55s ease-out;
  cursor: pointer;
}

.skills .iconfont__box:hover,
.iconfont__box.active {
  background: rgba(179, 181, 198, 1);
}

.skills .iconfont__box span {
  font-size: 16px;
}

.left .img {
  width: 100%;
  height: 100%;
  transition: all 0.55s ease-out;
}

.left .img:hover {
  filter: blur(4px);
}

.right {
  flex: 2;
  /* display: flex; */
  background: #f5f6fa;
  border-top-right-radius: 18px;
  padding: 20px 0;
  /* background: yellow; */
}

.iconfont {
  font-size: 32px;
}
</style>
