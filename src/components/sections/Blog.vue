<template>
  <section class="blog">
      <div class="container">
        <div class="blog__text">
            <div class="blog__text__title">
                farm to table
                <a href="#"><span>read our blog</span><i class="fas fa-book-reader"></i></a>
            </div>
            <div class="blog__text__subtitle">
                Aliquam erat voluptat. Ut quis ligula a magna blandit finibus. Suspendisse maximus lacus non nunc lacinia lobortis.
            </div>
        </div>

        <div class="post-section">

            <div class="col left">
                
                <div class="meal-card">
                    <a href="#"><img src="../../assets/img/single-post-img3.jpg" alt="sushi"></a>
                    <div class="text-card">
                        <div class="title">
                            Food Corner: Top Japanese Restaurants for Sushi
                        </div>
                        <div class="subtitle">
                            By admin I March 25th, 2019
                        </div>

                        <p>Lorem ipsum dolor sit amet, consectetur adipisicing elit. Ratione quaerat temporibus iste incidunt, fugiat ab harum debitis ullam itaque facilis sapiente ad repellendus officiis ipsam ducimus eligendi quod non facere.</p>

                        <div class="footer-card">
                            <a href="#"> <span>Read more</span><i class="fas fa-chevron-right"></i></a>
                            <a href="#"><i class="fas fa-comments"></i> <span>0</span></a>
                        </div>
                    </div>
  
                </div>

                <div class="meals-list">
                    
                    <div class="small-meal-card">
                        <a href="#"><img src="../../assets/img/fi-roundup.jpg" alt="roundup"></a>
                        <div class="text-card">
                            <div class="title">
                            Roundup: My New Favourite Recipes For Healthy Living
                            </div>
                            <div class="subtitle">
                            By admin I March 25th, 2019
                            </div>
                        </div>
                    </div>

                    <div class="small-meal-card">
                        <a href="#"><img src="../../assets/img/fi-korean-food.jpg" alt="korean food"></a>
                        <div class="text-card">
                            <div class="title">
                            Meal Prep: Korean Bibimbap with Kimchi
                            </div>
                            <div class="subtitle">
                            By admin I March 25th, 2019
                            </div>
                        </div>
                    </div>

                    <div class="small-meal-card">
                        <a href="#"><img src="../../assets/img/fi-toasts.jpg" alt="toats"></a>
                        <div class="text-card">
                            <div class="title">
                            Why These Toasts with Tea are My New Favourite
                            </div>
                            <div class="subtitle">
                            By admin I March 25th, 2019
                            </div>
                        </div>
                    </div>

                    <div class="small-meal-card">
                        <a href="#"><img src="../../assets/img/fi-street-food.jpg" alt="street food"></a>
                        <div class="text-card">
                            <div class="title">
                            Exploring Street Food in Bangkok
                            </div>
                            <div class="subtitle">
                            By admin I March 25th, 2019
                            </div>
                        </div>
                    </div>

                    <div class="small-meal-card">
                        <a href="#"><img src="../../assets/img/fi-organic-breakfast.jpg" alt="breakfast"></a>
                        <div class="text-card">
                            <div class="title">
                            Organic Choices For Healthier Living
                            </div>
                            <div class="subtitle">
                            By admin I March 25th, 2019
                            </div>
                        </div>
                    </div>

                    <div class="small-meal-card">
                        <a href="#"><img src="../../assets/img/fi-water-side-rest.jpg" alt="street food"></a>
                        <div class="text-card">
                            <div class="title">
                            5 Waterside Restaurants in Instanbul for Special Events
                            </div>
                            <div class="subtitle">
                            By admin I March 25th, 2019
                            </div>
                        </div>
                    </div>

                </div>

                <button>Load more posts</button>

            </div>

            <div class="col right">


                <!-- <a href="#">
                    <img class="menu" src="../../assets/img/ad-bg.jpg" alt="menu">
                    <div id="latest">view our latest recipes</div>
                </a> -->
                
            </div>

        </div>
      </div>
  </section>
</template>



<script>
export default {
    name: 'Blog'
}
</script>



<style lang="scss" scoped>
@import '../../assets/style/partials/variables.scss';

.blog{
    background-color: $mainBgColor;
    padding-bottom: 100px;
    &__text{
        padding: 80px 0;

        &__title{
            text-transform: uppercase;
            font-size: 25px;
            font-weight: bold;
            padding: 20px 0;
            display: flex;
            justify-content: space-between;

            a{
                text-decoration: none;
                color: white;
                background-color: $btnColor;
                padding: 10px 20px;
                border-radius: 5px;
                font-size: 16px;

                span{
                    margin-right: 15px;
                }

            }
        }

        &__subtitle{
            color: $contactColor;
            width: 40%;
            line-height:30px
        }
    }

    .post-section{
        display: flex;
        justify-content: space-between;

        .left{
            width: 63%;

            .meal-card{
                width: 100%;
                background-color: #fff;
            
                img{
                    width: 100%;
                }

                .text-card{
                    font-family: 'Orelega One', cursive;
                    margin: 0 auto;
                    padding: 40px;

                    .title{
                        font-size: 25px;
                        line-height: 40px;
                    }

                    .subtitle{
                        color: $contactColor;
                        line-height: 25px;
                        padding-bottom: 30px;
                    }

                    p{
                        border-top: 1px dotted $contactColor;
                        padding: 20px 0;
                        line-height: 30px;
                        color: $contactColor;
                    }

                    .footer-card{
                        display: flex;
                        justify-content: space-between;

                        a{
                            color: inherit;
                            text-decoration: none;
                        }

                        span{
                            font-size: 20px;
                            padding: 0 5px;
                        }
                    }
                }
            }

            .meals-list{
                width: 100%;
                display: flex;
                flex-wrap: wrap;
                justify-content: space-between;

                .small-meal-card{
                    width: 48%;
                    margin: 25px 0;
                    background-color: #fff;
            
                    img{
                        width: 100%;
                    }

                    .text-card{
                        font-family: 'Orelega One', cursive;
                        margin: 0 auto;
                        padding: 20px;
                        text-align: center;

                        .title{
                            font-size: 25px;
                            line-height: 40px;
                        }

                        .subtitle{
                            font-size: 15px;
                            line-height: 40px;
                            color: $contactColor;
                        }
                    }
                }
            }

            button{
                width: 100%;
                text-transform: uppercase;
                border: none;
                background-color: $secondBtnColor;
                color: $secondTextColor;
                font-size: 25px;
                padding: 10px;
                cursor: pointer;
            }
        }

        .right{
            width: 30%;
            
            // a{
            //     position: relative;
            // }

            // .menu{
            //     width: 100%;
            // }

            // #latest{
            //     position: absolute;
            //     top: 0;
            //     left: 0;
            // }

        }
    }
    
}
</style>