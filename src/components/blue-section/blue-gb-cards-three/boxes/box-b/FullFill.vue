<template>
    <div class="col-md-6 text-center">
        <div class="card dash-card p-2">
            <span>ls Fulfilled by Amazon</span>
            <canvas id="fulfill-chart" class="m-auto" height="100" width="100"></canvas>
        </div>
    </div>
</template>

<script>
import Chart from 'chart.js/auto';

export default {
    name: 'FullFill',
    components: {

    },
    mounted() {
        const ctx = document.getElementById('fulfill-chart')
        const data = {
            datasets: [{
                label: 'My First Dataset',
                data: [
                    { value: 75, name: "Search Engine" },
                    { value: 25, name: "Direct" },
                ],
                backgroundColor: [
                    '#55D8FE',
                    '#0946EC'
                ],
                hoverOffset: 4
            }]
        };

        const config = {
            type: 'doughnut',
            data: data,
        };

        const FullFillChart = new Chart(ctx, config)
        FullFillChart;

        console.log('FullFill was mounted!')

    }
}
</script>


<style scoped>
</style>