<script>
import AppHeader from './components/AppHeader.vue';
import AppFooter from './components/AppFooter.vue'
import AppMain from './components/AppMain.vue';
import AppJumbotron from './components/AppJumbotron.vue';

export default {
  components :{
    AppHeader,
    AppMain,
    AppFooter,
    AppJumbotron

  }
}

</script>

<template lang="">
  <div>
    <AppHeader></AppHeader>
    <AppJumbotron></AppJumbotron>
    <AppMain></AppMain>
    <AppFooter></AppFooter>
  </div>
</template>

<style lang="scss">
  @use './styles/generals.scss' as *;
</style>
