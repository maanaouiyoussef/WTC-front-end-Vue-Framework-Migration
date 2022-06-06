<template>
    <div class="col-md-6 text-center">
        <div class="card dash-card py-2 px-1">
            <span class='mb-3'>Connected to a Brand Store</span>
            <div id="brand-connection-chart">
                <div class="progress" style="max-height: 9px;">
                    <div class="progress-bar bg-sec" style="width: 20%;">
                    </div>
                    <div class="progress-bar bg-prim" style="width: 80%;">
                    </div>
                </div>
            </div>
        </div>
    </div>
</template>

<script>
export default {
    name: 'BrandConnection',
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