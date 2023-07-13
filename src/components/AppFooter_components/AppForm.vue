<script>
export default {

}
</script>

<template>
  <section id="form">
    <div>
      <h2>Subscribe <span>&</span> Receive A Free eBook</h2>
      <p class="text-center">Aliquam erat volutpat. Ut quis ligula a magna blandit finibus. Suspendisse maximus lacus non
        nunc lacinia
        lobortis.</p>
      <div class="d-flex align-items-center">
        <div class="pe-5">
          <input type="email" class="form-control" placeholder="insert your email...*">
        </div>
        <button type="submit" class="btn">SUBSCRIBE</button>
      </div>
    </div>
  </section>
  <section class="d-flex">
    <figure><img src="../../assets/img/Yogurt-Nan-400x263.jpg" alt="Yogurt Nan"></figure>
    <figure><img src="../../assets/img/Mixed-fruits-400x263.jpg" alt="Mixed Fruits"></figure>
    <figure><img src="../../assets/img/r-rachel-park-366508-unsplash-min-400x263.jpg" alt="Rachel Park"></figure>
    <figure><img src="../../assets/img/r-michelle-tsang-500721-unsplash-min-400x263.jpg" alt="Michelle Tsang"></figure>
  </section>
</template>

<style lang="scss" scoped>
@use '../../assets/scss/mixins.scss' as *;
@use '../../assets/scss/vars.scss' as *;

#form {
  height: 500px;
  margin-top: 80px;
  @include flex_center;
  background-image: url(../../assets/img/subscribe-sec-bg.png);
  background-position: center;
  background-repeat: no-repeat;
  background-size: cover;
  background-color: $primary-color;

  >div {
    height: 300px;
    width: 800px;
    background-color: $primary-color;
    @include flex_center;
    flex-direction: column;
  }
}

figure {
  width: 25%;
  height: 220px;
  margin: 0;

  img {
    object-fit: cover;
    height: 100%;
    width: 100%;
  }
}

h2 {
  font-family: Vidaloka;

  span {
    color: $secondary-color;
  }
}

p {
  padding: 20px 50px;
  color: $tertiary-color;
  font-size: 17px;
}

input {
  width: 500px;
}

button {
  background-color: $secondary-color;
  color: $primary-color;
  font-weight: 600;
  font-size: 14px;
  border-radius: 0;
  padding: 8px 20px;
  cursor: pointer;
}
</style>