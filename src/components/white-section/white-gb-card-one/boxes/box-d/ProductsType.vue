<template>
    <div class="col-md-8">
        <div class="card dash-card py-3 px-2">
            <span class="text-left">Products</span>
            <div id="products-type-chart" class='mt-3'>
                <div class="progress" style="max-height: 9px;">
                    <div class="progress-bar bg-prim" style="width: 80%;">
                    </div>
                    <div class="progress-bar bg-sec" style="width: 20%;">
                    </div>
                </div>
            </div>
        </div>
    </div>
</template>

<script>
export default {
    name: 'ProductsType',
    components: {

    }, 
    data() {
        return {
            
        }
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