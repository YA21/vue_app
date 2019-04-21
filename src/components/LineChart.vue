<script>
import { Line } from 'vue-chartjs'

export default {
    name: 'LineChart',
    extends: Line,
    props: ['data', 'title'],
    data () {
        return {
            chartData: {
                labels: ['1', '2', '3', '4'],
                datasets: [{
                    label: 'sample',
                    backgroundColor: '#0000ff',
                    data: []
                }]
            },
            options: {
                title: {
                    display: true,
                    text: ''
                },
                legend: {
                    display: false
                }
            }
        }
    },
    mounted: function() {
        this.chartData.datasets[0].data = this.data
        this.options.title.text = this.title
        this.renderChart(this.chartData, this.options)
    }
}

</script>