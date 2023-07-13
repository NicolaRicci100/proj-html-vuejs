<script>
import { gallery } from '../../data/index'
export default {
  methods: {
    getImagePath(imageFile) {
      const url = new URL(`/@/assets/img/${imageFile}`, import.meta.url);
      return url.href;
    }
  },
  data() {
    return {
      gallery
    }
  }
}
</script>

<template>
  <section id="journal" class="container shadow-lg">
    <div class="d-flex justify-content-center align-items-center">
      <span class="flex-grow-1"></span>
      <h5>FOODIE JOURNAL</h5>
      <span class="flex-grow-1"></span>
    </div>
    <div class="card-container row row-cols-3">
      <div class="col" v-for="item in gallery" :key="item.title">
        <div class="card text-center rounded-0 border-0">
          <img :src="getImagePath(item.foto)" class="card-img-top rounded-0" :alt="item.title">
          <div class="card-body">
            <h6 class="card-title">{{ item.title }}</h6>
            <p class="card-text">{{ item.text }}</p>
          </div>
        </div>
      </div>
    </div>
  </section>
</template>

<style lang="scss" scoped>
@use '../../assets/scss/mixins.scss' as *;
@use '../../assets/scss/vars' as *;

#journal {
  height: 450px;
  background-color: $primary-color;
  translate: 0 -80px;
}

span {
  background-color: gainsboro;
  height: 1px;
  margin: 0 50px;
}

h5 {
  @include flex_center;
  margin: 30px 0 20px;
}

h6 {
  font-family: Vidaloka;
  font-size: 22px;
  cursor: pointer;

  &:hover {
    color: $secondary-color;
  }
}

p {
  color: $tertiary-color;
}

.card-container {
  height: 370px;

  >div {
    @include flex_center;
  }
}
</style>