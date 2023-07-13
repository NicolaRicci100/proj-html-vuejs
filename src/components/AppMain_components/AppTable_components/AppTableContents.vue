<script>
export default {

}
</script>

<template>
  <div class="row">
    <div class="col-8">
      <div class="bg-white">
        Placeholder
      </div>
      <div>
        <ul class="row row-cols-2">
          <li class="col">Placeholder</li>
          <li class="col">Placeholder</li>
          <li class="col">Placeholder</li>
          <li class="col">Placeholder</li>
          <li class="col">Placeholder</li>
          <li class="col">Placeholder</li>
        </ul>
      </div>
    </div>
    <div class="col-4">
      Placeholder
    </div>
  </div>
</template>

<style lang="scss" scoped>
@use '../../../assets/scss/mixins.scss' as *;
@use '../../../assets/scss/vars' as *;

div.row {
  min-height: 2000px;
}

ul.row {
  min-height: 1200px;

  li {
    background-color: white;
    @include flex_center;
  }
}

div.bg-white {
  height: 800px;
}
</style>