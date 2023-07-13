<script>
import AppJournal from './AppMain_components/AppJournal.vue';
import AppRecipies from './AppMain_components/AppRecipies.vue';
import AppCollection from './AppMain_components/AppCollection.vue';
import AppTable from './AppMain_components/AppTable.vue';
export default {
  components: { AppJournal, AppRecipies, AppCollection, AppTable }
}
</script>

<template>
  <section id="jumbotron">
    <div>
      <div class="shadow-lg">TODAY'S PICKS</div>
      <h2>Food Corner: Top Japanese Restaurants for Sushi</h2>
      <span>March 25, 2019</span>
    </div>
  </section>
  <AppJournal />
  <AppRecipies />
  <AppCollection />
  <!-- <AppTable /> -->
</template>

<style lang="scss" scoped>
@use '../assets/scss/mixins.scss' as *;
@use '../assets/scss/vars.scss' as *;


#jumbotron {
  height: 600px;
  @include flex_center;
  background-image: url(../assets/img/single-post-img3-1200x790.jpg);
  background-position: center;
  background-repeat: no-repeat;
  background-size: cover;

  >div {
    height: 200px;
    width: 700px;
    background-color: $primary-color;
    @include flex_center;
    flex-direction: column;
    border-radius: 5px;

    >div {
      translate: 0 -15px;
      color: $primary-color;
      background-color: $secondary-color;
      padding: 8px 16px;
      border-radius: 5px;
      font-weight: 600;
    }
  }
}

h2 {
  padding: 10px 100px;
  text-align: center;
  font-family: Vidaloka;
  font-size: 40px;
  cursor: pointer;

  &:hover {
    color: $secondary-color;
  }
}

span {
  color: $tertiary-color;
  padding-bottom: 20px;
}
</style>