<script>
export default {

}
</script>

<template>
  <section class="bg-white">
    <div class="container">
      <div class="row">
        <div class="col">Placeholder</div>
        <div class="col">Placeholder</div>
        <div class="col">Placeholder</div>
        <div class="col">Placeholder</div>
      </div>
    </div>
  </section>
  <footer>
    Placeholder
  </footer>
</template>

<style lang="scss" scoped>
@use '../../assets/scss/mixins.scss' as *;
@use '../../assets/scss/vars' as *;

section {
  padding: 50px 0 50px;
}

div.row {
  height: 400px;
}

footer {
  height: 90px;
  @include flex_center;
  border: $debug;
}
</style>