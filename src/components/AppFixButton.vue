<script>
export default {

}
</script>

<template>
  <section>
    <div class="shadow-lg">
      <i class="fa-solid fa-boxes-stacked d-block pb-1"></i>
      Prebuilts
    </div>
    <div class="shadow-lg">
      <i class="fa-solid fa-cart-shopping d-block pb-1"></i>
      Buy Now
    </div>
  </section>
</template>

<style lang="scss" scoped>
@use '../assets/scss/mixins.scss' as *;
@use '../assets/scss/vars.scss' as *;

section {
  position: fixed;
  z-index: 1;
  top: 200px;
  right: 0;

  div {
    height: 66px;
    width: 66px;
    margin: 20px;
    background-color: $primary-color;
    color: $tertiary-color;
    @include flex_center;
    flex-direction: column;
    cursor: pointer;
    border-radius: 10px;
    font-weight: 600;

    &:hover {
      color: $secondary-color;
    }
  }
}
</style>