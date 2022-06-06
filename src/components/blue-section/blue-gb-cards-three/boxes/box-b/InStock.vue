<template>
    <div class="col-md-6 text-center">
        <div class="card dash-card p-2">
            <span>In Stock?</span>
            <canvas id="instock-chart" class="m-auto" height="60" width="60"></canvas>
        </div>
    </div>
</template>

<script>
import { Chart } from 'chart.js';


export default {
    name: 'InStock',
    components: {

    }, 
    mounted() {
        const ctx = document.getElementById('instock-chart')
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

        console.log('InStock was mounted!')

    }
}
</script>


<style scoped>
</style>