<script>
import Line from 'vue-chartjs'

export default {
    name: 'LineChart',
    extends: Line,
    data: function() {
        return {
            data: {
                labels: ['1', '2', '3', '4'],
                datasets: [{
                    label: 'sample',
                    backgroundColor: '#0000ff',
                    data: [100, 90, 60, 70]
                }]
            },
            options: {
                responsive: false,
                maintainAspectRatio: false
            }
        }
    },
    mounted: function() {
        console.log("hoge")
        this.renderChart(this.data, this.options)
    }
}

</script>

<style>
</style>