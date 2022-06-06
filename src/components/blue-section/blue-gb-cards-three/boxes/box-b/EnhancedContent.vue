<template>
    <div class="col-md-6 text-center">
        <div class="card dash-card p-2">
            <span>Enhanced Content</span>
            <canvas id="enhanced-chart" class="m-auto" height="60" width="60"></canvas>
        </div>
    </div>
</template>

<script>
import { Chart } from 'chart.js';


export default {
    name: 'EnhancedContent',
    components: {

    }, 
    mounted() {
        const ctx = document.getElementById('enhanced-chart')
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

        const inStockChart = new Chart(ctx, config)
        inStockChart;

        console.log('EnhancedContent was mounted!')

    }
}
</script>


<style scoped>
</style>