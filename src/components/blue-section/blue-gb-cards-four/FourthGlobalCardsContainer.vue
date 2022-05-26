<template>
    <div id="fourth-global-cards-container">
        <!-- Title -->
        <div class="card-title mb-2">
            <strong>CUSTOMER REVIEWS</strong>
        </div>
        <div class="card card-body p-4">
            <div class="row">
                <BoxOne />
                <BoxTwo />
                <BoxThree />
                <BoxFour />
            </div>
        </div>
    </div>


</template>

<script>
import BoxOne from './boxes/box-a/BoxOne.vue';
import BoxTwo from './boxes/box-b/BoxTwo.vue';
import BoxThree from './boxes/box-c/BoxThree.vue';
import BoxFour from './boxes/box-d/BoxFour.vue';
export default {
    name: 'FourthGlobalCardsContainer',
    components: {
        BoxOne,
        BoxTwo,
        BoxThree,
        BoxFour
    }
}
</script>


<style scoped>
#fourth-global-cards-container {
    width: 1000px;
}

.dash-card {
    font-size: 11px;
    border: 1px solid #0946ec;
}
</style>