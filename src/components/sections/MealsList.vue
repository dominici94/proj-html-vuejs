<template>
  <section class="meals-list">

      <div class="meal-card">
          <img src="../../assets/img/Yogurt-Nan.jpg" alt="yogurt">
      </div>

      <div class="meal-card">
          <img src="../../assets/img/Mixed-fruits.jpg" alt="fruits">
      </div>

      <div class="meal-card">
          <img src="../../assets/img/r-rachel-park-366508-unsplash-min.jpg" alt="breakfast">
      </div>

      <div class="meal-card">
          <img src="../../assets/img/r-michelle-tsang-500721-unsplash-min.jpg" alt="icecream">
      </div>
  </section>
</template>

<script>
export default {
    name: 'MealList'
}
</script>

<style lang="scss" scoped>
@import '../../assets/style/partials/variables.scss';

.meals-list{
    display: flex;

    .meal-card{
        width: calc(100% / 4);

        img{
            width: calc(100%);
        }
    }
}





</style>