<template>
    <div class="col-md-6 text-center">
        <div class="card dash-card py-2 px-1">
            <span class='mb-3'>With Video in the Gallery</span>
            <div id="video-in-gallery-chart">
                <div class="progress" style="max-height: 9px;">
                    <div class="progress-bar bg-sec" style="width: 90%;">
                    </div>
                    <div class="progress-bar bg-prim" style="width: 10%;">
                    </div>
                </div>
            </div>
        </div>
    </div>
</template>

<script>
export default {
    name: 'VideoInGallery',
    props: {

    },
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