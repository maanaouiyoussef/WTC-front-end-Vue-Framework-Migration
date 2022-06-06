<template>
    <!-- Second Column -->
    <div class="col-md-8">
        <span style="font-weight: bold">RETAILER-SPECIFIC BADGES</span>
        <div class="card px-3">
            <div class="row g-3 text-center">
                <div class="col-md-4">
                    <span style="font-size: 10px">Is Amazon Choice </span>
                    <div id="amazon-choice-chart">
                        <div class="progress" style="max-height: 9px;">
                            <div class="progress-bar bg-prim" style="width: 90%;">
                            </div>
                            <div class="progress-bar bg-sec" style="width: 10%;">
                            </div>
                        </div>
                    </div>
                </div>
                <div class="col-md-4">
                    <span style="font-size: 10px">Has Subscribe And Save option</span>
                    <div id="subs-chart" class='mb-3'>
                        <div class="progress" style="max-height: 9px;">
                            <div class="progress-bar bg-prim" style="width: 90%;">
                            </div>
                            <div class="progress-bar bg-sec" style="width: 10%;">
                            </div>
                        </div>
                    </div>
                </div>
                <div class="col-md-4">
                    <span style="font-size: 10px">Climate Pledge Friendly</span>
                    <div id="climate-chart">
                        <div class="progress" style="max-height: 9px;">
                            <div class="progress-bar bg-prim" style="width: 90%;">
                            </div>
                            <div class="progress-bar bg-sec" style="width: 10%;">
                            </div>
                        </div>
                    </div>
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
.bg-prim {
    background-color: #0946EC;
}

.bg-sec {
    background-color: #55D8FE;
}
</style>