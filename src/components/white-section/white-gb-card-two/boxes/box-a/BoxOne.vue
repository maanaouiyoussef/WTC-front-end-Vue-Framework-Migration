<template>
    <!-- First Column -->
    <div class="col-md-4 recommandation-box">
        <span style="font-weight: bold">MEDICAL LABEL</span>
        <div class="card p-1">
            <div class="container">
                <span style="font-size: 10px">Is Recommended by Dermatologists</span>
                <div id="dermato-recommandation-chart">Line CHart</div>
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
</style>