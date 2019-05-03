<template>
    <div style='display:flex;'>
        <line-chart 
            class=chart
        />
        <bar-chart
            class=chart
        />
        <pie-chart
            class=chart
        />
    </div>
</template>

<script>
import LineChart from './LineChart'
import BarChart from './BarChart'
import PieChart from './PieChart'

export default {
    components: { LineChart, BarChart, PieChart },
}
</script>

<style>
.chart {
    width: 500px;
    height: 500px;
}
</style>
