<template>
    <!-- First Global Cards Container Start -->
    <div id="first-global-cards-container" class="card card-body p-4 mb-3">
        <!-- Title + Logo -->
        <div id="headline">
            <img class="headline-logo" src="../../../assets/img/Logo.png" alt="" />
            <div class="headline-title"><strong>KEY FINDINGS</strong></div>
        </div>

        <div class="row g-4">
            <BoxOne />
            <BoxTwo />
            <BoxThree />
            <BoxFour />
        </div>
    </div>
</template>

<script>
import BoxOne from "./boxes/box-a/BoxOne.vue";
import BoxTwo from "./boxes/box-b/BoxTwo.vue";
import BoxThree from "./boxes/box-c/BoxThree.vue";
import BoxFour from "./boxes/box-d/BoxFour.vue";


export default {
    name: 'FirstGlobalCardsContainer',
    components: {
    BoxOne,
    BoxTwo,
    BoxThree,
    BoxFour
}
}
</script>


<style scoped>
/* First Global Cards Container */
#first-global-cards-container {
  position: relative;
  width: 1000px;
  height: 95%;
  z-index: 12;
}
/* Headline */
#headline {
  position: absolute;
  top: 0%;
  left: 0%;
  right: 0%;
  bottom: 0%;
  margin: -120px;
  z-index: 1; 
}

.headline-logo {
  color: #353535;
  font-size: 16pt;
  letter-spacing: 3px;
  text-transform: uppercase;
}

.headline-title {
  font-size: 16pt;
  display: inline-block;
  margin-top: -50px;
}
</style>