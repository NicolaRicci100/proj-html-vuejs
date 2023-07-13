<script>
export default {

}
</script>

<template>
  <section class="bg-white">
    <div class="container">
      <div class="row">
        <div class="col border-end d-flex flex-column justify-content-center">
          <img class="mb-5" src="../../assets/img/avada-food-logo-mob-2x.png" alt="Avada Logo">
          <div>
            <i class="fa-brands fa-facebook-f"></i>
            <i class="fa-brands fa-instagram"></i>
            <i class="fa-brands fa-twitter"></i>
            <i class="fa-brands fa-youtube"></i>
          </div>
        </div>
        <div class="col border-end d-flex align-items-center">
          <ul>
            <li>Recipes</li>
            <li>Places</li>
            <li>Blog</li>
            <li>About</li>
            <li>Contact</li>
          </ul>
        </div>
        <div class="col border-end d-flex flex-column align-itms-center justify-content-center">
          <h6>CONTACT US</h6>
          <div class="d-flex py-4">
            <i class="fa-solid fa-location-dot pe-4"></i>
            <div>775 New York Ave, Brooklyn, Kings, New York 11203</div>
          </div>
          <div class="d-flex py-4">
            <i class="fa-solid fa-phone pe-4"></i>
            <div>+ 0100-505-0000</div>
          </div>
          <div class="d-flex py-4">
            <i class="fa-solid fa-envelope pe-4"></i>
            <div>info@your-domain.com</div>
          </div>
        </div>
        <div class="col d-flex flex-column align-itms-center justify-content-center">
          <h6 class="pb-4">GET OUR APP</h6>
          <img class="py-4 ps-4" src="../../assets/img/download-app-store.png" alt="App store">
          <img class="py-4 ps-4" src="../../assets/img/download-android.png" alt="Android store">
        </div>
      </div>
    </div>
  </section>
  <footer>
    <div>© Copyright 2012 - 2019 | Avada Website Builder by ThemeFusion | All Rights Reserved | Powered by WordPress</div>
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
}

img {
  width: 85%;
}

i {
  cursor: pointer;
  padding: 4px 8px;
  border-radius: 5px;
  color: $tertiary-color;
  font-size: 20px;

  &:hover {
    color: $secondary-color;
  }
}

ul li {
  font-size: 18px;
  font-weight: 600;
  line-height: 50px;
  padding-left: 30px;
  cursor: pointer;

  &:hover {
    color: $secondary-color;
  }
}

h6 {
  color: $secondary-color;
  font-weight: 600;
}
</style>