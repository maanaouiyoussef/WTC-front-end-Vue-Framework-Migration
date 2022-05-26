<template>
  <NavBar />
  <WhiteSection />
  <BlueSection />
</template>

<script>
import NavBar from './components/NavBar.vue';
import WhiteSection from './components/white-section/WhiteSection.vue';
import BlueSection from './components/blue-section/BlueSection.vue';

export default {
  name: 'App',
  components: {
    NavBar,
    WhiteSection,
    BlueSection
}
}
</script>

<style>
#app {
 
}

.dash-card {
  font-size: 11px;
  border: 1px solid #0946ec;
}
</style>
