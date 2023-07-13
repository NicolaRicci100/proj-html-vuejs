<script>
export default {
  methods: {
    getImagePath(imageFile) {
      const url = new URL(`/@/assets/img/${imageFile}`, import.meta.url);
      return url.href;
    }
  },
  data() {
    return {
      foods: [
        'Mixed-fruits-400x263.jpg',
        'r-rachel-park-366508-unsplash-min-400x263.jpg',
        'r-michelle-tsang-500721-unsplash-min-400x263.jpg',
        'quick-summer-drink-460x295.jpg',
        'r-maarten-van-den-heuvel-400626-unsplash-min-460x295.jpg',
        'perfect-cosmopolitan-460x295.jpg',
        'fi2x-6-460x295.jpg',
        'r-brooke-lark-96398-unsplash-min-460x295.jpg'
      ]
    }
  }
}
</script>

<template>
  <section class="container">
    <div class="row justify-content-center">
      <div class="col-8">
        <h5>POPULAR RECIPES</h5>
        <p class="text-center">Aliquam erat volutpat. Ut quis ligula a magna blandit finibus. Suspendisse maximus
          lacus
          non nunc lacinia
          lobortis.</p>
      </div>
      <div class="col-6 bg-white card p-0 border-0 rounded-0">
        <img src="../../assets/img/Yogurt-Nan-800x527.jpg" class="card-img-top rounded-0 border-0" alt="Yogurt-Nan">
        <div class="card-body">
          <h5 class="card-title">Lunch Favourite with Salad, Naan And Beans</h5>
          <span>Bakery, Featured, Healthy, Latest Recipes, Staff Picks</span>
          <p class="card-text">Suspendisse at semper odio. Nam fringilla scelerisque tincidunt. Orci varius natoque
            penatibus et magnis dis parturient montes, nascetur ridiculus mus. Donec tincidunt posuere ornare. Phasellus
            placerat odio non feugiat sollicitudin. Integer vitae elementum ex. Sed porttitor, diam eget convallis
            volutpat, arcu tellus facilisis nulla, id dignissim orci leo id</p>
          <a href="#" class="btn">LEARN MORE</a>
        </div>
      </div>
      <div class="col-6">
        <div class="d-flex flex-wrap justify-content-evenly">
          <figure v-for="food in foods" :key="food"><img :src="getImagePath(food)" :alt="food"></figure>
        </div>
      </div>
    </div>
  </section>
</template>

<style lang="scss" scoped>
@use '../../assets/scss/mixins.scss' as *;
@use '../../assets/scss/vars.scss' as *;

section {
  height: 1000px;
}

.row {
  height: 100%;
}

.col-8 {
  height: 20%;
  @include flex_center;
  flex-direction: column;

  p {
    padding: 30px 150px 0;
    color: $tertiary-color;
    font-size: 17px;
  }
}

.card {
  h5 {
    font-family: Vidaloka;
    padding-top: 30px;
    cursor: pointer;

    &:hover {
      color: $secondary-color;
    }
  }

  p {
    padding: 50px 0;
  }

  a {
    background-color: $secondary-color;
    color: $primary-color;
    font-weight: 600;
    font-size: 14px;
    border-radius: 0;
  }
}

.col-6 {
  height: 80%;
  @include flex_center('main');
}

figure {
  height: 160px;
  width: 250px;
  @include flex_center;

  img {
    width: 100%;
  }
}
</style>