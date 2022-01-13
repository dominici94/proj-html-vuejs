<template>
  <section class="meals-list">

      <div class="meal-card">
          <div class="meal-img">
                    <a href="#"><img src="../../assets/img/Yogurt-Nan.jpg" alt="yogurt"></a>
                    <div class="hover-meal">
                        <div class="icon">
                            <i class="fas fa-link"></i>
                         </div>
                        Lunch Favourite with Salad, Naan And Beans
                    </div>
            </div>
          <!-- <img src="../../assets/img/Yogurt-Nan.jpg" alt="yogurt"> -->
      </div>

      <div class="meal-card">
          <div class="meal-img">
                    <a href="#"><img src="../../assets/img/Mixed-fruits.jpg" alt="fruits"></a>
                    <div class="hover-meal">
                        <div class="icon">
                            <i class="fas fa-link"></i>
                         </div>
                        Fruit Platter with Banana, Mango, Berries and Orange
                    </div>
            </div>
          <!-- <img src="../../assets/img/Mixed-fruits.jpg" alt="fruits"> -->
      </div>

      <div class="meal-card">
          <div class="meal-img">
                    <a href="#"><img src="../../assets/img/r-rachel-park-366508-unsplash-min.jpg" alt="breakfast"></a>
                    <div class="hover-meal">
                        <div class="icon">
                            <i class="fas fa-link"></i>
                         </div>
                        Waffle with Banana, Berries and Strawberries
                    </div>
            </div>
          <!-- <img src="../../assets/img/r-rachel-park-366508-unsplash-min.jpg" alt="breakfast"> -->
      </div>

      <div class="meal-card">
          <div class="meal-img">
                    <a href="#"><img src="../../assets/img/r-michelle-tsang-500721-unsplash-min.jpg" alt="icecream"></a>
                    <div class="hover-meal">
                        <div class="icon">
                            <i class="fas fa-link"></i>
                         </div>
                        IceCream
                    </div>
            </div>
          <!-- <img src="../../assets/img/r-michelle-tsang-500721-unsplash-min.jpg" alt="icecream"> -->
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

        .meal-img{
                    width: 100%;
                    position: relative;

                    a{
                        display: grid;
                    }

                    img{
                        width: 100%;
                    }

                    .hover-meal{
                        display: none;
                        width: 100%;
                        height: 100%;
                        position: absolute;
                        top: 0;
                        left: 0;
                        background: linear-gradient(to bottom, rgba(133, 67, 15, 0.5) 0%,$btnColor 100%);
                        overflow: auto;
                        padding: 30px;
                        color: white;

                        .icon{
                            padding: 10px;
                            border-radius: 50%;
                            background-color: white;
                            color: rgba($color: #000000, $alpha: 0.5);
                        }
                    }
            }
            
            .meal-img:hover .hover-meal{
                display: flex;
                flex-direction: column;
                justify-content: center;
                align-items: center;
            }
        img{
            width: calc(100%);
        }
    }
}





</style>