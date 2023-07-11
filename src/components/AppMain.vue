<script>
import AppJournal from './AppMain_components/AppJournal.vue';
import AppRecipies from './AppMain_components/AppRecipies.vue';
export default {
  components: { AppJournal, AppRecipies }
}
</script>

<template>
  <section id="jumbotron">
    <div>
      Placeholder
    </div>
  </section>
  <AppJournal />
  <AppRecipies />
</template>

<style lang="scss" scoped>
@use '../assets/scss/mixins.scss' as *;
@use '../assets/scss/vars.scss' as *;


#jumbotron {
  height: 600px;
  @include flex_center;

  // temporanei
  background-image: url(../assets/img/3a74ce3d0532b7773b174c45ca3bd05a_bigger.png);
  border: $debug;

  >div {
    height: 200px;
    width: 700px;
    background-color: $primary-color;
    @include flex_center;
  }
}
</style>