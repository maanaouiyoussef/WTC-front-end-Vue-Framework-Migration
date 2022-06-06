<template>
    <!-- First Column -->
    <div class="col-md-4 recommandation-box">
        <span style="font-weight: bold">MEDICAL LABEL</span>
        <div class="card px-3">
            <div class="container">
                <span style="font-size: 10px">Is Recommended by Dermatologists</span>
                <div id="dermato-recommandation-chart" class="mb-3">
                    <div class="progress" style="max-height: 9px;">
                        <div class="progress-bar bg-prim" style="width: 40%;">
                        </div>
                        <div class="progress-bar bg-sec" style="width: 60%;">
                        </div>
                    </div>
                </div>
            </div>
        </div>
    </div>
    <!-- First Column End-->
</template>

<script>
export default {
    name: 'BoxOne',
    components: {

    }
}
</script>


<style scoped>
.recommandation-box {
    z-index: 5;
}
.bg-prim {
    background-color: #0946EC;
}

.bg-sec {
    background-color: #55D8FE;
}
</style>