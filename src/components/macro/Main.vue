<template>
  <main>
      <FoodieJournal/>
      <PopularRecipes/>
      <CulinaryCollection/>
  </main>
</template>

<script>
import FoodieJournal from '../sections/FoodieJournal.vue';
import PopularRecipes from '../sections/PopularRecipes.vue';
import CulinaryCollection from '../sections/CulinaryCollection.vue';

export default {
    name: 'Main',
    components: {
      FoodieJournal,
      PopularRecipes,
      CulinaryCollection
    }
}
</script>

<style>

</style>