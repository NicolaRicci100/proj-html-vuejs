<script>
export default {
  data() {
    return {
      menu: [
        'Home',
        'Recipes',
        'Places',
        'Blog',
        'About',
        'Contact',
      ]
    }
  }
}
</script>

<template>
  <section class="container">
    <div class="row row-cols-3 justify-content-center">
      <div class="col d-flex justify-content-start align-items-start pt-3">
        <a href="#">Download App <span class="d-inline">iOS</span></a>
        <a href="#" class="ps-4">Advertise with us</a>
      </div>
      <div class="col logo">
        <img src="../assets/img/avada-food-logo.png" alt="logo di Avada Food">
      </div>
      <div class="col d-flex justify-content-end align-items-start pt-3">
        <i class="fa-brands fa-facebook-f"></i>
        <i class="fa-brands fa-instagram"></i>
        <i class="fa-brands fa-twitter"></i>
        <i class="fa-brands fa-youtube"></i>
      </div>
      <div class="col-6" id="menu-nav">
        <span v-for="voice in menu">{{ voice }}</span>
        <span><i class="fa-solid fa-magnifying-glass"></i></span>
      </div>
    </div>
  </section>
</template>

<style lang="scss" scoped>
@use '../assets/scss/mixins.scss' as *;
@use '../assets/scss/vars' as *;

.row {
  height: 200px;
  color: $tertiary-color;
}

a {
  font-size: 13px;
  font-weight: 500;

  span {
    background-color: $secondary-color;
    color: $primary-color;
    padding: 0 8px;
    border-radius: 5px;
  }

}

.logo {
  @include flex_center;

  img {
    cursor: pointer;
  }

}

div>i {
  cursor: pointer;
  padding: 4px 8px;
  border-radius: 5px;

  &:hover {
    background-color: $primary-color;
  }
}

#menu-nav {
  @include flex_center('cross');
  justify-content: space-between;

  span {
    cursor: pointer;
    font-weight: 600;

    &:hover {
      color: $secondary-color;
    }
  }
}
</style>