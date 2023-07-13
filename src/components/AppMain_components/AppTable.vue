<script>
import AppTableContents from './AppTable_components/AppTableContents.vue';
export default {
  components: { AppTableContents }
}
</script>

<template>
  <section class="container">
    <div class="row">
      <div class="col d-flex justify-content-start flex-column">
        <h5>FARM TO TABLE</h5>
        <p>Aliquam erat volutpat. Ut quis ligula a magna blandit finibus. Suspendisse maximus lacus
          non nunc lacinia lobortis.</p>
      </div>
      <div class="col d-flex justify-content-end align-items-start">
        <a href="#">READ OUR BLOG <i class="fa-solid fa-book-open-reader ps-2"></i></a>
      </div>
    </div>
    <AppTableContents />
  </section>
</template>

<style lang="scss" scoped>
@use '../../assets/scss/mixins.scss' as *;
@use '../../assets/scss/vars' as *;

section {
  margin-top: 80px;

  >div {
    height: 150px;
  }
}

.row>div {

  p {
    padding: 20px 0;
    color: $tertiary-color;
    font-size: 17px;
  }
}

a {
  background-color: $secondary-color;
  color: $primary-color;
  font-weight: 600;
  font-size: 14px;
  border-radius: 0;
  padding: 8px 20px;
  cursor: pointer;
}
</style>