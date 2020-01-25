<template>
  <div>
    <apexchart width="500" type="bar" :options="chartOptions" :series="series"></apexchart>
  </div>
</template>

<script>
export default {
  data: function() {
    return {
      chartOptions: {
        chart: {
          id: "ブクログ読書記録"
        },
        plotOptions: {
          bar: {
            horizontal: false,
            endingShape: "rounded",
            dataLabels: {
              position: "top"
            }
          }
        },
        dataLabels: {
          position: "top",
          offsetY: -20,
          style: {
            colors: ["#1E1E1E"]
          }
        },
        tooltip: {
          enabled: false
        },
        xaxis: {
          categories: [
            "1月",
            "2月",
            "3月",
            "4月",
            "5月",
            "6月",
            "7月",
            "8月",
            "9月",
            "10月",
            "11月",
            "12月"
          ]
        },
        colors: ["#4EA6CC"]
      },
      series: [
        {
          name: "冊数",
          data: [16, 14, 68, 44, 12, 24, 7, 16, 18, 0, 7, 5]
        }
      ]
    };
  }
};
</script>
