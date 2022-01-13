<template>
    <section class="foodie">

        <div class="foodie__journal container">

            <div class="foodie__journal__title">
                <hr>
                <h2>foodie journal</h2>
                <hr>
            </div>
            

            <div class="meal-list">

                <!-- meal card riutilizzabile -->
                <div class="meal-card">

                    <div class="meal-img">
                        <a href="#"><img src="../../assets/img/single-post-img3.jpg" alt="sushi"></a>
                        <div class="hover-meal">
                            <div class="icon">
                                <i class="fas fa-link"></i>
                            </div>
                            Food Corner: Top Japanese Restaurants for Sushi
                        </div>
                    </div>
                    
                    <div class="text-card">
                        <div class="title">
                            Food Corner: Top Japanese Restaurants for Sushi
                        </div>
                        <div class="subtitle">
                            By admin I March 25th, 2019
                        </div>
                    </div>
                </div>

                <div class="meal-card">

                    <div class="meal-img">
                        <a href="#"><img src="../../assets/img/fi-roundup.jpg" alt="roundup"></a>
                        <div class="hover-meal">
                            <div class="icon">
                                <i class="fas fa-link"></i>
                            </div>
                            Roundup: My New Favourite Recipes For Healthy Living
                        </div>
                    </div>
                    
                    <div class="text-card">
                        <div class="title">
                            Roundup: My New Favourite Recipes For Healthy Living
                        </div>
                        <div class="subtitle">
                            By admin I March 25th, 2019
                        </div>
                    </div>
                </div>

                <div class="meal-card">

                    <div class="meal-img">
                        <a href="#"><img src="../../assets/img/fi-toasts.jpg" alt="toasts"></a>
                        <div class="hover-meal">
                            <div class="icon">
                                <i class="fas fa-link"></i>
                            </div>
                            Why These Toasts with Tea are My New Favourite
                        </div>
                    </div>
                    
                    <div class="text-card">
                        <div class="title">
                            Why These Toasts with Tea are My New Favourite
                        </div>
                        <div class="subtitle">
                            By admin I March 25th, 2019
                        </div>
                    </div>
                </div>
                
            </div>

        </div>

    </section>
</template>

<script>
export default {
    name: 'FoodieJournal'
}
</script>

<style lang='scss' scoped>
@import '../../assets/style/partials/variables.scss';

.foodie{
    background-color: $mainBgColor;
    

    &__journal{
        background-color: white;
        padding: 40px 20px;
        text-align: center;
        transform: translateY(-20%);
        box-shadow: $mainShadow;

        &__title{
            width: 100%;
            display: flex;
            align-items: center;
            justify-content: center;

            hr{
                width: calc(35% - 25px);
                border: 1px dotted $contactColor;
                display: inline-block;
            }

            h2{
                text-transform: uppercase;
                display: inline-block;
                width: 30%;
            }
        }
        

        .meal-list{
            width: 100%;
            display: flex;
            margin-top: 50px;

            .meal-card{
                width: calc(100% / 3 - 50px);
                margin: 0 25px;

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
            
                .text-card{
                    font-family: 'Orelega One', cursive;
                    margin: 0 auto;
                    padding: 20px;

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
        
    }
}

</style>