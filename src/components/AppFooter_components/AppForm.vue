<script>
export default {

}
</script>

<template>
  <section id="form">
    <div>
      Placeholder
    </div>
  </section>
  <section class="d-flex">
    <figure>Placeholder</figure>
    <figure>Placeholder</figure>
    <figure>Placeholder</figure>
    <figure>Placeholder</figure>
  </section>
</template>

<style lang="scss" scoped>
@use '../../assets/scss/mixins.scss' as *;
@use '../../assets/scss/vars.scss' as *;

#form {
  height: 500px;
  margin-top: 80px;
  @include flex_center;

  // temporanei
  background-image: url(../../assets/img/3a74ce3d0532b7773b174c45ca3bd05a_bigger.png);
  border: $debug;

  >div {
    height: 300px;
    width: 800px;
    background-color: $primary-color;
    @include flex_center;
  }
}

figure {
  width: 25%;
  height: 220px;
  border: $debug;
  margin: 0;
}
</style>