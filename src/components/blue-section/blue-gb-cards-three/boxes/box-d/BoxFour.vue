<template>
    <!-- Column Four Start-->
    <div class="col-md-3">

        <DataTable />

        <!-- Download - Rank  Start -->
        <div class="row">
            <div class="col-md-8" style="font-size: 11px">
                Rank tracking is available by clicking the right picture
            </div>
            <div class="col-md-4">
                <a href="#">
                    <img id="download-icon" src="../../../../../assets/img/DownloadReport.png" width="65" height="35"
                        alt="" />
                </a>
            </div>
        </div>
        <!-- Download - Rank  End -->
    </div>
    <!-- Column Four ENd-->
</template>

<script>
import DataTable from './DataTable.vue'
export default {
    name: 'BoxFour',
    components: {
        DataTable
    }
}
</script>


<style scoped>
.download-icon {
    cursor: pointer;
}
</style>