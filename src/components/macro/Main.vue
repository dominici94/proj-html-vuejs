<template>
  <main>
      <FoodieJournal/>
      <PopularRecipes/>
      <CulinaryCollection/>
      <Blog/>
      <Subscribe/>
  </main>
</template>

<script>
import FoodieJournal from '../sections/FoodieJournal.vue';
import PopularRecipes from '../sections/PopularRecipes.vue';
import CulinaryCollection from '../sections/CulinaryCollection.vue';
import Blog from '../sections/Blog.vue';
import Subscribe from '../sections/Subscribe.vue';

export default {
    name: 'Main',
    components: {
      FoodieJournal,
      PopularRecipes,
      CulinaryCollection,
      Blog,
      Subscribe
    }
}
</script>

<style>

</style>