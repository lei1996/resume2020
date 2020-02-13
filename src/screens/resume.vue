<template>
  <div class="container">
    <div class="left">
      <div class="header-portrait">
        <div class="img_box">
          <img class="img" src="../assets/logo.png" alt="" />
        </div>
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
    <div class="right">2</div>
  </div>
</template>

<script>
import RadarComponent from "../components/Radar.vue";
// import LineComponent from "../components/Line.vue";

export default {
  //   props: {
  //     msg: String
  //   }
  components: {
    RadarComponent
    // LineComponent,
  },
  data() {
    return {
      barWidth: "50",
      radarData: {
        labels: [
          "Angular",
          "React",
          "Vue.js",
          "Flutter",
          "Jquery",
          "linux",
          "asd"
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
            data: [75, 20, 85, 51, 68, 45, 27]
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
  margin-top: 40px;
  background: #fff;
  display: flex;
}

.left {
  flex: 1;
  /* background: red; */
  padding-bottom: 80px;
  display: flex;
  justify-content: center;
  align-items: center;
  flex-direction: column;
  position: relative;
}

.left .img_box:hover {
    box-shadow: 4px 4px 8px rgba(148, 145, 145, .6);
}
.left .img_box {
  background: #fff;
  border-radius: 6px;
  width: 150px;
  height: 150px;
  overflow: hidden;
  box-shadow: 4px 4px 8px rgba(148, 145, 145, .3);
  transition: all 0.25s ease-out;
  cursor: pointer;
  /* border: 4px solid #545050; */
  position: absolute;
  left: -40px;
  top: -40px;
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
  background: yellow;
}

.iconfont {
  font-size: 32px;
}
</style>
