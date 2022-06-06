<template>
    <div class="col-md-4 text-center">
        <div class="card dash-card p-1">
            <span>Always ON?</span>
            <canvas id="availibiliy-check-chart" class="mx-auto mt-0" height="50" width="50"></canvas>
        </div>
    </div>
</template>

<script>
import Chart from 'chart.js/auto'

export default {
    name: 'AlwaysON',
    components: {

    },
    mounted() {
        const ctx = document.getElementById('availibiliy-check-chart')
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

        const alwaysOnChart = new Chart(ctx, config)
        alwaysOnChart;
    }
}

</script>


<style scoped>
</style>