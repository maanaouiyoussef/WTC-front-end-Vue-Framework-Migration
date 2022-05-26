<template>
    <!-- Column One -->
    <div class="col-md-3 card-one">
        <div class="alert alert-primary m-0 py-1 px-3 my-1" role="alert">
            <strong>99.85%</strong> have a title &lt;200 chars
        </div>
        <div class="alert m-0 py-1 px-3 my-1" role="alert">
            <strong>50.3%</strong> have 6 images or more
        </div>
        <div class="alert alert-primary m-0 py-1 px-3 my-1" role="alert">
            <strong>7.43%</strong> have a video
        </div>
        <div class="alert m-0 py-1 px-3 my-1" role="alert">
            <strong>29.99%</strong> have bullet points >100 chars
        </div>
        <div class="alert alert-primary m-0 py-1 px-3 my-1" role="alert">
            <strong>72.58%</strong> are connected to a Brand Store
        </div>
        <div class="alert m-0 py-1 px-3 my-1" role="alert">
            <strong>76.81%</strong> are inside a variation
        </div>
    </div>
    <!-- Column One END-->
</template>

<script>
export default {
    name: 'BoxOne',
    components: {

    }
}
</script>

<style scoped>
.alert {
    color: black;
    font-size: 12px;
    border: none;
    border-radius: 2px;
}

.alert.alert-primary {
    background-color: #c4e2f0;
}
</style>