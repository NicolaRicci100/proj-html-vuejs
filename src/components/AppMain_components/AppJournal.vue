<script>
export default {

}
</script>

<template>
  <section id="journal" class="container">
    <h4>Placeholder</h4>
    <div class="card-container row row-cols-3">
      <div class="col">Placeholder</div>
      <div class="col">Placeholder</div>
      <div class="col">Placeholder</div>
    </div>
  </section>
</template>

<style lang="scss" scoped>
@use '../../assets/scss/mixins.scss' as *;
@use '../../assets/scss/vars' as *;

#journal {
  height: 450px;
  background-color: $primary-color;
  border: $debug; //temporaneo
}

h4 {
  @include flex_center;
  margin: 30px 0 20px;
}

.card-container {
  height: 370px;

  >div {
    @include flex_center;
  }
}
</style>