<template>
    <div class="col-md-6 text-center">
        <div class="card dash-card p-2">
            <span>Pictures</span>
            <canvas id="pictures-chart" class='m-auto' height="100" width="100"></canvas>
        </div>
    </div>
</template>

<script>
import Chart from 'chart.js/auto'
export default {
    name: 'PicturesChart',
    components: {

    },
    mounted() {
        const ctx = document.getElementById('pictures-chart')
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

        const picturesChart = new Chart(ctx, config)
        picturesChart;
    }
}
</script>


<style scoped>
</style>