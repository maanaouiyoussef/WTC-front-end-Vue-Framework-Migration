<template>
    <!-- Global Cards Container Two Start -->
    <div class="row" id="second-global-cards-container">
        <BoxOne />
        <BoxTwo />
    </div>
    <!-- Global Cards Container Two End -->
</template>

<script>
import BoxTwo from './boxes/box-b/BoxTwo.vue';
import BoxOne from './boxes/box-a/BoxOne.vue';
export default {
    name: 'SecondGlobalCardsContainer',
    components: {
        BoxTwo,
        BoxOne
    }
}
</script>

<style scoped>
#second-global-cards-container {
  width: 1024px;
}
</style>