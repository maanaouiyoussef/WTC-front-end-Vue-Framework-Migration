<template>
    <div class="col-md-6 text-center">
        <div class="card dash-card p-2">
            <span>Bulletpoints</span>
            <canvas id='bulletPoints' class="m-auto" height="100" width="100"></canvas>
        </div>
    </div>
</template>

<script>

import Chart from 'chart.js/auto'

export default {
    name: 'BulletPoints',
    components: {

    },
    mounted() {
        const ctx = document.getElementById('bulletPoints')
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

        const bulletPointsChart = new Chart(ctx, config)
        bulletPointsChart;
    }
}
</script>


<style scoped>
</style>