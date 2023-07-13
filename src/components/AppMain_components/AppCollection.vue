<script>
import { collections } from '../../data/index'
export default {
  methods: {
    getImagePath(imageFile) {
      const url = new URL(`/@/assets/img/${imageFile}`, import.meta.url);
      return url.href;
    }
  },
  data() {
    return {
      collections
    }
  }
}
</script>

<template>
  <section class="container">
    <div>
      <h5>CULINARY COLLECTION</h5>
      <p class="text-center">Aliquam erat volutpat. Ut quis ligula a magna blandit finibus. Suspendisse maximus lacus non
        nunc lacinia lobortis.</p>
    </div>
    <ul class="row row-cols-4">
      <!-- <li class="col d-flex flex-column" v-for="item in collections" :key="item.name">
        <img src="../../assets/img/drinks-recipes.png" :alt="item.name">
        <p>{{ item.name }}</p>
      </li> -->
      <li class="col d-flex flex-column">
        <img src="../../assets/img/drinks-recipes.png">
        <p>DRINKS</p>
      </li>
      <li class="col d-flex flex-column">
        <img src="../../assets/img/soups-recipes.png">
        <p>SOUPS</p>
      </li>
      <li class="col d-flex flex-column">
        <img src="../../assets/img/baking-recipes.png">
        <p>BAKERY</p>
      </li>
      <li class="col d-flex flex-column">
        <img src="../../assets/img/dinner-recipes.png">
        <p>DINNER</p>
      </li>
      <li class="col d-flex flex-column">
        <img src="../../assets/img/healthy-recipes.png">
        <p>HEALTHY</p>
      </li>
      <li class="col d-flex flex-column">
        <img src="../../assets/img/staff-picks.png">
        <p>STAFF PICKS</p>
      </li>
      <li class="col d-flex flex-column">
        <img src="../../assets/img/premium-recipes.png">
        <p>APPETISER</p>
      </li>
      <li class="col d-flex flex-column">
        <img src="../../assets/img/quick-easy-recipes.png">
        <p>QUICK & EASY</p>
      </li>
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
    flex-direction: column;

    p {
      padding: 30px 300px 0;
      color: $tertiary-color;
      font-size: 17px;
    }
  }
}

ul {
  height: calc(100% / 3 * 2);
}

li {
  height: 50%;
  @include flex_center;
  background-color: $primary-color;
  border: 20px solid $bg-color;

  img {
    height: 50%;
  }

  p {
    font-weight: 600;
    padding-top: 20px;
  }
}
</style>