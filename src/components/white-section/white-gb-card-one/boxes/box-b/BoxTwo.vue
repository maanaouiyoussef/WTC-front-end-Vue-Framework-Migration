<template>
    <!-- Column Two -->
    <div class="col-md-4 border-start border-primary">
        <!-- First Row-->
        <div class="row g-2">
            <Bulletpoints />
            <PicturesChart />
        </div>
        <!-- First Row End-->

        <!-- Second Row-->
        <div class="row g-2 mt-1">
            <VideoInGallery />
            <BrandConnection />
        </div>
        <!-- Second Row End-->
    </div>
    <!-- Column Two END -->
</template>

<script>
import PicturesChart from './PicturesChart.vue'
import Bulletpoints from './Bulletpoints.vue'
import BrandConnection from './BrandConnection.vue'
import VideoInGallery from './VideoInGallery.vue'

export default {
    name: 'BoxTwo',
    components: {
    PicturesChart,
    Bulletpoints,
    BrandConnection,
    VideoInGallery
}
}
</script>


<style scoped>
</style>