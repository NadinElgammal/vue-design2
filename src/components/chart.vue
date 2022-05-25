<template>
  <div>
    <div id="main"></div>
  </div>
</template>

<script>
import * as echarts from "echarts";
export default {
  name: "Chart",
  methods: {
    drawChart() {
      var chartDom = document.getElementById("main");
      var myChart = echarts.init(chartDom);
      var option;

      option = {
        color: ["#F00",'#0164FB'],
        xAxis: {
          type: "category",
          data: ["Mon", "Tue", "Wed", "Thu", "Fri", "Sat", "Sun","Mon", "Tue", "Wed", "Thu", "Fri", "Sat", "Sun" ,"Mon", "Tue", "Wed", "Thu", "Fri", "Sat"],
        },
        yAxis: {
          type: "value",
        },
        series: [
          {
            data: [100, 165, 222, 142, 120, 111, 235 , 200 ,100, 165, 222, 142, 120, 111, 235 , 200 ,100, 165, 222, 142, 120, 111],
            type: "line",
          },
          {
            data: [33, 105, 212, 152, 250, 122, 215 , 260 ,110, 135, 202, 142, 120, 111, 235 , 122 ,110, 135, 202],
            type: "line",
          },
        ],
      };
      option && myChart.setOption(option);
    },
  },
  mounted() {
    this.drawChart();
  },
};
</script>
<style scoped>
#main{
  width: 100%;
  height: 400px;
}
</style>
