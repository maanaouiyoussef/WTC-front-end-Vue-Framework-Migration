<template>
    <section id='white-section'>
        <FirstGlobalCardsContainer />
        <SecondGlobalCardsContainer />
    </section>
</template>

<script>
import FirstGlobalCardsContainer from './white-gb-card-one/FirstGlobalCardsContainer.vue';
import SecondGlobalCardsContainer from './white-gb-card-two/SecondGlobalCardsContainer.vue';
export default {
    name: 'WhiteSection',
    components: {
    FirstGlobalCardsContainer,
    SecondGlobalCardsContainer
}
}
</script>

<style scoped>
/* Section One: White BG */
#white-section {
  display: flex;
  flex-direction: column;
  align-items: center;
  justify-content: space-around;
  width: 100%;
  height: 490px;
  background: linear-gradient(
      0deg,
      rgba(218, 216, 217, 0.26),
      rgba(209, 207, 208, 0.26)
    ),
    url("../../assets/img/BubblesWhiteBG.png");
  padding: 100px 0px 30px 0;
}
</style>