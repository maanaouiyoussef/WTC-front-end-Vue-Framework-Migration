<template>
  <!-- Column Four Start-->
  <div class="col-md-3">
    <!-- First Row-->
    <div class="row g-2 mb-2">
      <div class="col text-center">
        <div class="card dash-card p-2">
          <!-- Two Sub Columns -->
          <div class="row">
            <SelectedProducts />
            <LastUpdate />
          </div>
        </div>
      </div>
    </div>
    <!-- First Row End-->

    <!-- Second Row-->
    <div class="row g-2 mb-2">
      <ProductsType />
      <AlwaysON />
    </div>
    <!-- Second Row End-->

    <!-- Third Row-->
    <MedContentScoreValue />
    <!-- Third Row End-->
  </div>
  <!-- Column Four End -->
</template>

<script>
import SelectedProducts from './SelectedProducts.vue';
import LastUpdate from './LastUpdate.vue';
import ProductsType from './ProductsType.vue';
import AlwaysON from './AlwaysON.vue';
import MedContentScoreValue from './MedContentScoreValue.vue';
export default {
  name: 'BoxFour',
  components: {
    SelectedProducts,
    LastUpdate,
    ProductsType,
    AlwaysON,
    MedContentScoreValue
  }
}
</script>


<style scoped>
</style>