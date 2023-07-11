<script>
import AppTableContents from './AppTable_components/AppTableContents.vue';
export default {
  components: { AppTableContents }
}
</script>

<template>
  <section class="container">
    <div class="row">
      <div class="col d-flex justify-content-start">Placeholder</div>
      <div class="col d-flex justify-content-end">Placeholder</div>
    </div>
    <AppTableContents />
  </section>
</template>

<style lang="scss" scoped>
@use '../../assets/scss/mixins.scss' as *;

section {
  margin-top: 80px;

  >div {
    height: 150px;
  }
}
</style>