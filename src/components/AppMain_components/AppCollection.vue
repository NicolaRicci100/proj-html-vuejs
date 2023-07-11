<script>
export default {

}
</script>

<template>
  <section class="container">
    <div>Placeholder</div>
    <ul class="row row-cols-4">
      <li class="col">Placeholder</li>
      <li class="col">Placeholder</li>
      <li class="col">Placeholder</li>
      <li class="col">Placeholder</li>
      <li class="col">Placeholder</li>
      <li class="col">Placeholder</li>
      <li class="col">Placeholder</li>
      <li class="col">Placeholder</li>
    </ul>
  </section>
</template>

<style lang="scss" scoped>
@use '../../assets/scss/mixins.scss' as *;
@use '../../assets/scss/vars.scss' as *;

section {
  height: 600px;
  margin-top: 80px;

  div {
    height: calc(100% / 3);
    @include flex_center;
  }
}

ul {
  height: calc(100% / 3 * 2);
}

li {
  height: 50%;
  border: $debug;
  @include flex_center;
  background-color: $primary-color;
}
</style>