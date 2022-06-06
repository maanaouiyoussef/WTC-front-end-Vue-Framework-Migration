<template>
    <!-- Column Two Start -->
    <div class="col-md-3 text-center border-start border-primary">
        <div class="card dash-card p-2">
            <span style="font-size: 11px"> Reviews count </span>
            <canvas id="reviews-count-chart" class="m-auto" height="180" width="180"></canvas>
        </div>
    </div>
    <!-- Column Two End-->
</template>

<script>
import Chart from 'chart.js/auto'
export default {
    name: 'BoxTwo',
    components: {

    },
    mounted() {
        const ctx = document.getElementById('reviews-count-chart')
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
            type: 'pie',
            data: data,
        };

        const reviewsCountChart = new Chart(ctx, config)
        reviewsCountChart;

        console.log('Reviews Count was mounted!')
    }
}
</script>


<style scoped>
</style>