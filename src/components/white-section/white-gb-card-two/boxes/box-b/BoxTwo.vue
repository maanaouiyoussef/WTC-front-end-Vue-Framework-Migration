<template>
    <!-- Second Column -->
    <div class="col-md-8">
        <span style="font-weight: bold">RETAILER-SPECIFIC BADGES</span>
        <div class="card p-1">
            <div class="row g-3 text-center">
                <div class="col-md-4">
                    <span style="font-size: 10px">Is Amazon Choice </span>
                    <div id="amazon-choice-chart">Line CHart</div>
                </div>
                <div class="col-md-4">
                    <span style="font-size: 10px">Has Subscribe And Save option</span>
                    <div id="subs-chart">Line CHart</div>
                </div>
                <div class="col-md-4">
                    <span style="font-size: 10px">Climate Pledge Friendly</span>
                    <div id="climate-chart">Line CHart</div>
                </div>
            </div>
        </div>
    </div>
    <!-- Second Column End-->
</template>

<script>
export default {
    name: 'BoxTwo',
    components: {

    }
}
</script>


<style scoped>
</style>