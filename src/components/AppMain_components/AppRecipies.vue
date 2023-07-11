<script>
export default {

}
</script>

<template>
  <section class="container">
    <div class="row justify-content-center">
      <div class="col-8">
        Placeholder
      </div>
      <div class="col-6">
        Placeholder
      </div>
      <div class="col-6">
        Placeholder
      </div>
    </div>
  </section>
</template>

<style lang="scss" scoped>
@use '../../assets/scss/mixins.scss' as *;
@use '../../assets/scss/vars' as *;

section {
  height: 1000px;
}

.row {
  height: 100%;
}

.col-8 {
  height: 20%;
  @include flex_center;
}

.col-6 {
  height: 80%;
  @include flex_center;
}
</style>