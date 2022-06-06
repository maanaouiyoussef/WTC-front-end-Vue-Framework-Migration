<template>
    <!-- Column Three Start -->
    <div class="col-md-3 text-center">
        <div class="card dash-card p-2">
            <span style="font-size: 11px"> Reviews Rating </span>
            <canvas id="reviews-rating-chart" class="m-auto" height="180" width="180"></canvas>
        </div>
    </div>
    <!-- Column Three End-->

</template>

<script>
import Chart from 'chart.js/auto'
export default {
    name: 'BoxThree',
    components: {

    },
     mounted() {
        const ctx = document.getElementById('reviews-rating-chart')
        const data = {
            datasets: [{
                label: 'My First Dataset',
                data: [
                    { value: 25, name: "Search Engine" },
                    { value: 75, name: "Direct" },
                ],
                backgroundColor: [
                    '#0946EC','#55D8FE'
                ],
                hoverOffset: 4
            }]
        };

        const config = {
            type: 'pie',
            data: data,
        };

        const reviewsRatingChart = new Chart(ctx, config)
        reviewsRatingChart;

        console.log('Reviews Rating Chart was mounted!')
    }
}
</script>


<style scoped>
</style>