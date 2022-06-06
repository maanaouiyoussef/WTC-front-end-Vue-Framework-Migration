<template>
    <!-- Column Four Start -->
    <div class="col-md-3 text-center">
        <div class="card dash-card p-2">
            <span style="font-size: 11px"> % of new reviews added from the last month </span>
            <canvas id="new-reviews-chart" class="m-auto" height="162" width="162"></canvas>
        </div>
    </div>
    <!-- Column Four End-->
</template>

<script>
import Chart from 'chart.js/auto'

export default {
    name: 'BoxFour',
    components: {

    },
    mounted() {
        const ctx = document.getElementById('new-reviews-chart')
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

        const newReviewsChart = new Chart(ctx, config)
        newReviewsChart;

        console.log('newReviews was mounted!')
    }
}

</script>


<style scoped>
</style>