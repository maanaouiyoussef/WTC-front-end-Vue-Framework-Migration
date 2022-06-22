<template>
    <div class="col-md-6">
        <span>Selected Products</span>
        <div id="products-count">{{ productsCount }}</div>
    </div>
</template>

<script>
export default {
    name: 'SelectedProducts',
    components: {

    },
    data() {
        return {
            productsCount: 355.61,
        }
    }
}
</script>


<style scoped>
#products-count {
    font-size: 13pt;
    color: #0946ec;
    font-weight: bold;
}
</style>