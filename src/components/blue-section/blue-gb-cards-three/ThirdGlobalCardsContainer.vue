<template>
    <div id="third-global-cards-container" class="card card-body p-4 mb-3">
        <!-- Ice Container-->
        <!-- <div id='iceberg'>
            <img src="../../../assets/img/Iceberg.png">
        </div> -->

        <div class="row g-4">
            <Iceberg />
            <BoxOne />
            <BoxTwo />
            <BoxThree />
            <BoxFour />
        </div>
    </div>
</template>

<script>
import BoxOne from './boxes/box-a/BoxOne.vue';
import BoxTwo from './boxes/box-b/BoxTwo.vue';
import BoxThree from './boxes/box-c/BoxThree.vue';
import BoxFour from './boxes/box-d/BoxFour.vue';
import Iceberg from './Iceberg.vue';
export default {
    name: 'ThirdGlobalCardsContainer',
    components: {
    BoxOne,
    BoxTwo,
    BoxThree,
    BoxFour,
    Iceberg
}
}
</script>

<style>
#third-global-cards-container {
  position: relative;
  width: 1000px;
}

.alert {
  color: black;
  font-size: 12px;
  border: none;
  border-radius: 2px;
}

.alert.alert-primary {
  background-color: #c4e2f0;
}

.dash-card {
  font-size: 11px;
  border: 1px solid #0946ec;
}

#iceberg {
    position: absolute;
    margin: -184px;
    z-index: -1;
}
</style>