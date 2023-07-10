<script>
import AppHeader from './components/AppHeader.vue';
import AppMain from './components/AppMain.vue';
export default {
  components: { AppHeader, AppMain }
}
</script>

<template>
  <AppHeader />
  <AppMain />
</template>

<style lang="scss">
@use './assets/scss/style.scss' as *;
@use './assets/scss/vars.scss' as *;
@use './assets/scss/mixins.scss' as *;

// debug temporaneo
section {
  div {
    border: $debug;
  }
}
</style>