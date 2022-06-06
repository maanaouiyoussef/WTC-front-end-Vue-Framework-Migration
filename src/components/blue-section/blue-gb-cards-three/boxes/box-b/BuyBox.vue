<template>
    <div class="col-md-6 text-center">
        <div class="card dash-card p-2 p-2">
            <span>Buy Box is Amazon</span>
            <canvas id="buybox-chart" class="m-auto" height="100" width="100"></canvas>
        </div>
    </div>
</template>

<script>
import Chart from 'chart.js/auto';

export default {
    name: 'BuyBox',
    components: {

    },
    mounted() {
        const ctx = document.getElementById('buybox-chart')
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

        const buyBoxChart = new Chart(ctx, config)
        buyBoxChart;

        console.log('BuyBox was mounted!')
    }
}
</script>


<style scoped>
</style>