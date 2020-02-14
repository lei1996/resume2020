<template>
  <div id="app">
    <!-- <img alt="Vue logo" src="./assets/logo.png" /> -->
    <!-- <HelloWorld msg="Welcome to Your Vue.js App" /> -->
    <Resume />
    <!-- <LineComponent :barWidth="barWidth" />
    <span class="iconfont icon-duanxin"></span>
    <RadarComponent class="radar" :radarData="radarData" :options="options" /> -->
  </div>
</template>

<script>
// import HelloWorld from "./components/HelloWorld.vue";
// import RadarComponent from "./components/Radar.vue";
// import LineComponent from "./components/Line.vue";
import Resume from "./screens/resume.vue";

export default {
  name: "App",
  components: {
    // HelloWorld,
    // RadarComponent,
    // LineComponent,
    Resume
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
            label: "各项技能能力值",
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

<style>
@import "./assets/styles/iconfont.css";
.radar {
  background: #fff;
  width: 200px;
  height: 200px;
}

#app {
  font-family: Avenir, Helvetica, Arial, sans-serif;
  -webkit-font-smoothing: antialiased;
  -moz-osx-font-smoothing: grayscale;
  text-align: center;
  color: #2c3e50;
  background: #e5e8ed;
  display: flex;
  justify-content: center;
  align-items: center;
  min-height: 100vh;
}
html,
body,
* {
  margin: 0;
  padding: 0;
  box-sizing: border-box;
}
a {
  list-style: none;
}
</style>
