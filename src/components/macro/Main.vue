<template>
  <main>
      <FoodieJournal/>
      <PopularRecipes/>
  </main>
</template>

<script>
import FoodieJournal from '../sections/FoodieJournal.vue';
import PopularRecipes from '../sections/PopularRecipes.vue';
export default {
    name: 'Main',
    components: {
      FoodieJournal,
      PopularRecipes,
    }
}
</script>

<style>

</style>