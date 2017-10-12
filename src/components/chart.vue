<template>
    <chartist
        ratio="ct-major-second"
        type="Line"
        :data="chartData"
        :options="chartOptions" >
    </chartist>
</template>

<script>
      export default({ 
        name: 'chart',
        data () {
            return {
                chartData: {
                    labels: ["A", "B", "C"],
                    series:[[1, 3, 2], [4, 6, 5]]
                },
                chartOptions: {
                    lineSmooth: false
                }
            }
        }
      })
</script>
<style lang="scss">
    
</style>