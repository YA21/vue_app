<template>
    <div id="app">
        <line-chart
            :data='data'
            :title='title'
        />
    </div>
</template>

<script>
import LineChart from './LineChart'

export default {
    components: { LineChart },
    data () {
        return {
            data: [100, 90, 60, 70],
            title: 'line-chart'
        }
    }
}
</script>

<style>
#app {
    font-family: 'Avenir', Helvetica, Arial, sans-serif;
    -webkit-font-smoothing: antialiased;
    -moz-osx-font-smoothing: grayscale;
    text-align: center;
    color: #2c3e50;
    margin-top: 60px;
}
</style>
