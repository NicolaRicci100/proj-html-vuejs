<script>
import AppHeader from './components/AppHeader.vue';
export default {
  components: { AppHeader }
}
</script>

<template>
  <AppHeader />
</template>

<style lang="scss">
@use './assets/scss/style.scss' as *;
@use './assets/scss/vars.scss' as *;

// debug temporaneo
section div {
  border: $debug;
}
</style>