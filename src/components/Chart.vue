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
          id: "vuechart-example"
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
        }
      },
      series: [
        {
          name: "series-1",
          data: [30, 40, 35, 50, 49, 60, 70, 91, 10, 20, 12, 13]
        }
      ]
    };
  }
};
</script>
