<script>
export default {

}
</script>

<template>
  <section class="container">
    <div class="row row-cols-3 justify-content-center">
      <div class="col">Placeholder</div>
      <div class="col text-center">Placeholder</div>
      <div class="col text-end">Placeholder</div>
      <div class="col-6 text-center">Placeholder</div>
    </div>
  </section>
</template>

<style lang="scss" scoped>
@use '../assets/scss/mixins.scss' as *;

//temporaneo
.row {
  height: 200px;

  :last-child {
    @include flex_center
  }
}
</style>