<template>
  <section class="popular">

    <div class="container">

        <div class="popular__text">
            <div class="popular__text__title">
                popular recipes
            </div>
            <div class="popular__text__subtitle">
                Aliquam erat voluptat. Ut quis ligula a magna blandit finibus. Suspendisse maximus lacus non nunc lacinia lobortis.
            </div>
        </div>

        <div class="popular__meals">

            <div class="popular__meals__col left">

                <div class="meal-img">
                        <a href="#"><img src="../../assets/img/Yogurt-Nan.jpg" alt="yogurt"></a>
                        <div class="hover-meal">
                            <div class="icon">
                                <i class="fas fa-link"></i>
                            </div>
                            Lunch Favourite with Salad, Naan And Beans
                        </div>
                </div>



                <div class="popular__meals__col__text">
                    <div class="title">
                        <h3>Lunch Favourite with Salad, Naan And Beans</h3>
                        <h5>Bakery, Featured, Healthy, Latest Recipes, Staff Picks</h5>
                        <p>Lorem ipsum dolor sit amet consectetur adipisicing elit. Accusantium, magnam. Commodi eveniet maiores ad in quos incidunt sequi alias, ipsam quidem vel, ipsa ea culpa repellendus reiciendis doloribus dolores molestias!</p>
                    </div>
                    
                    <a href="#">learn more</a>
                </div>

            </div>
            
            <div class="popular__meals__col right">
                <div class="card-image">
                    <img src="../../assets/img/Mixed-fruits.jpg" alt="fruits">
                </div>
                <div class="card-image">
                    <img src="../../assets/img/r-rachel-park-366508-unsplash-min.jpg" alt="waffle">
                </div>
                <div class="card-image">
                    <img src="../../assets/img/r-michelle-tsang-500721-unsplash-min.jpg" alt="icecream">
                </div>
                <div class="card-image">
                    <img src="../../assets/img/quick-summer-drink-460x295.jpg" alt="drink">
                </div>
                <div class="card-image">
                    <img src="../../assets/img/r-maarten-van-den-heuvel-400626-unsplash-min-460x295.jpg" alt="colorfood">
                </div>
                <div class="card-image">
                    <img src="../../assets/img/perfect-cosmopolitan-460x295.jpg" alt="cosmopolitan">
                </div>
                <div class="card-image">
                    <img src="../../assets/img/fi2x-6-460x295.jpg" alt="fruits and vegetables">
                </div>
                <div class="card-image">
                    <img src="../../assets/img/r-brooke-lark-96398-unsplash-min-460x295.jpg" alt="sweet">
                </div>
            </div>

        </div>

    </div>
      
  </section>
</template>

<script>
export default {
    name: 'PopularRecipes'

}
</script>

<style lang='scss' scoped>
@import '../../assets/style/partials/variables.scss';

.popular{
    background-color: $mainBgColor;

    &__text{
        text-align: center;

        &__title{
            text-transform: uppercase;
            font-size: 25px;
            font-weight: bold;
            padding: 20px 0;
        }

        &__subtitle{
            color: $contactColor;
            width: 40%;
            margin: 0 auto;
            line-height:30px
        }
    }

    &__meals{
        display: flex;
        justify-content: space-between;
        margin-top: 70px;

        &__col{
            width: 48%;

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

            &__text{
                padding: 40px;

                .title{
                    margin-bottom: 20px;
                    
                    h3{
                        font-family: 'Orelega One', cursive;
                        font-weight: lighter;
                        line-height: 25px;
                    }

                    h5{
                        line-height: 25px;
                        padding-bottom: 30px;
                    }

                    p{
                        border-top: 1px dotted $contactColor;
                        padding: 20px 0;
                        line-height: 30px;
                    }
                }

                a{
                    color: white;
                    background-color: $btnColor;
                    text-decoration: none;
                    padding: 10px 20px;
                }
            }
            
        }

        .left{
            background-color: #fff;
            box-shadow: $mainShadow;
        }

        .right{
            display: flex;
            flex-wrap: wrap;
            justify-content: space-between;

            .card-image{
                width: 48%;
                margin-bottom: 20px;

                img{
                    width: 100%;
                    height: 160px;
                    object-fit: cover;
                }
            }
        }
    }
}

</style>