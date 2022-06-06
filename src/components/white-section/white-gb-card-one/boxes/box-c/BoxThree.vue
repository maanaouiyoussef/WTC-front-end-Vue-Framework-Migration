<template>
    <!-- Column Three Start -->
    <div class="col-md-2 text-center">
        <span style="font-size: 11px">Count of prodkey by with questions and answer status</span>
        <canvas id="prodkey-qa-chart" height="100" width="100" class="mt-2"></canvas>
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
        const prodKey = document.getElementById('prodkey-qa-chart')
        const pkData = {
            labels: [],
            datasets: [
                {
                    label: "My First Dataset",
                    data: [300, 100],
                    backgroundColor: ["#55D8FE", "#0946EC"],
                    hoverOffset: 4,
                },
                {
                    label: "My First Dataset",
                    data: [300, 100],
                    backgroundColor: ["#55D8FE", "#D72D4E"],
                    hoverOffset: 4,
                },
            ],
        };

        const pkConfig = {
            type: "doughnut",
            data: pkData,
        };

        const pkChart = new Chart(prodKey, pkConfig, {
            title: {
                text: "Doughnut Chart",
                verticalAlign: "center",
                dockInsidePlotArea: true
            }
        });
        pkChart;
    }
}
</script>


<style scoped>
</style>