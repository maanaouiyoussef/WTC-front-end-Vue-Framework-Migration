<template>
    <!-- Column Two -->
    <div class="col-md-4 border-start border-primary">
        <!-- First Row-->
        <div class="row g-2">
            <BuyBox />
            <FullFill />
        </div>

        <!-- First Row End-->

        <!-- Second Row-->
        <div class="row g-2 mt-1">
            <InStock />
            <EnhancedContent />
        </div>
    </div>
    <!-- Second Row End-->
    <!-- Column Two END -->
</template>

<script>

import BuyBox from './BuyBox.vue'
import FullFill from './FullFill.vue'
import InStock from './InStock.vue'
import EnhancedContent from './EnhancedContent.vue'


export default {
    name: 'BoxTwo',
    components: {
    BuyBox,
    FullFill,
    InStock,
    EnhancedContent
}
}
</script>


<style scoped>
</style>