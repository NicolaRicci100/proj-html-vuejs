<script>
export default {

}
</script>

<template>
  <section id="jumbotron">
    <div>
      Placeholder
    </div>
  </section>
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

  div {
    height: 200px;
    width: 700px;
    background-color: $bg-color;
    @include flex_center;
  }
}
</style>