<template>
    <!-- Column Three Start -->
    <div class="col-md-2 text-center">
        <span style="font-size: 11px"> Medical content SCORE </span>
        <canvas id="medical-content-chart" class="mt-2"></canvas>
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
        const ctx = document.getElementById('medical-content-chart')
        // Medical Content Score CHart
        const mdContentScoreData = {
            labels: [],
            datasets: [
                {
                    label: "My First Dataset",
                    data: [300, 100],
                    backgroundColor: ["#55D8FE", "#0946EC"],
                    hoverOffset: 4,
                    cutout: '0%'
                },
                {
                    label: "My First Dataset",
                    data: [300, 100],
                    backgroundColor: ["#55D8FE", "#D72D4E"],
                    hoverOffset: 4,
                    cutout: '0%'
                },
                {
                    label: "My First Dataset",
                    data: [300, 100],
                    backgroundColor: ["#55D8FE", "#D72D4E"],
                    hoverOffset: 4,
                    cutout: '0%'
                },
                {
                    label: "My First Dataset",
                    data: [300, 100],
                    backgroundColor: ["#55D8FE", "#D72D4E"],
                    hoverOffset: 4,
                    cutout: '0%'
                },
            ],
        };

        const mdConfig = {
            type: "doughnut",
            data: mdContentScoreData,
        };

        const mdChart = new Chart(ctx, mdConfig);
        mdChart; 
    }
}
</script>

<style scoped>
#third-global-cards-container {
    position: relative;
    width: 1000px;
}
#medical-content-chart {
    
}
</style>