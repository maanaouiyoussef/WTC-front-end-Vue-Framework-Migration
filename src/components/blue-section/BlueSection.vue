<template>
   <section id="blue-section">
       <ThirdGlobalCardsContainer />
       <FourthGlobalCardsContainer />
   </section>
</template>

<script>
import ThirdGlobalCardsContainer from './blue-gb-cards-three/ThirdGlobalCardsContainer.vue';
import FourthGlobalCardsContainer from './blue-gb-cards-four/FourthGlobalCardsContainer.vue';
export default {
    name: 'BlueSection',
    components: {
    ThirdGlobalCardsContainer,
    FourthGlobalCardsContainer
}
}
</script>

<style scoped>
/* Section Two: Blue BG */
#blue-section {
  display: flex;
  flex-direction: column;
  justify-content: space-around;
  align-items: center;
  background-image: url("../../assets/img/BubblesBlueBG.png");
  background-size: cover;
  background-position: middle;
  width: 100%;
  max-height: 890px;
  padding: 20px;
}
</style>