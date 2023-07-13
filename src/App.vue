<script>
import AppHeader from './components/AppHeader.vue';
import AppMain from './components/AppMain.vue';
import AppFooter from './components/AppFooter.vue';
import AppFixButton from './components/AppFixButton.vue';
export default {
  components: { AppHeader, AppMain, AppFooter, AppFixButton }
}
</script>

<template>
  <AppFixButton />
  <AppHeader />
  <AppMain />
  <AppFooter />
</template>

<style lang="scss">
@use './assets/scss/style.scss' as *;
@use './assets/scss/vars.scss' as *;
@use './assets/scss/mixins.scss' as *;
</style>