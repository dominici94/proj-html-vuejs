<template>
  <section class="culinary">
      <div class="container">

        <div class="culinary__text">
            <div class="culinary__text__title">
                culinary collection
            </div>
            <div class="culinary__text__subtitle">
                Aliquam erat voluptat. Ut quis ligula a magna blandit finibus. Suspendisse maximus lacus non nunc lacinia lobortis.
            </div>
        </div>

        <div class="list-icon">

            <div class="card-icon">
                <a href="#"><img src="../../assets/img/drinks-recipes.png" alt="drink"></a>
                <div class="text">
                    <a href="#">drinks</a>
                </div>
            </div>
            
            <div class="card-icon">
                <a href="#"><img src="../../assets/img/soups-recipes.png" alt="drink"></a>
                <div class="text">
                    <a href="#">soups</a>
                </div>
            </div>

            <div class="card-icon">
                <a href="#"><img src="../../assets/img/baking-recipes.png" alt="drink"></a>
                <div class="text">
                    <a href="#">bakery</a>
                </div>
            </div>

            <div class="card-icon">
                <a href="#"><img src="../../assets/img/dinner-recipes.png" alt="drink"></a>
                <div class="text">
                    <a href="#">dinner</a>
                </div>
            </div>

            <div class="card-icon">
                <a href="#"><img src="../../assets/img/healthy-recipes.png" alt="drink"></a>
                <div class="text">
                    <a href="#">healthy</a>
                </div>
            </div>

            <div class="card-icon">
                <a href="#"><img src="../../assets/img/staff-picks.png" alt="drink"></a>
                <div class="text">
                    <a href="#">staff picks</a>
                </div>
            </div>

            <div class="card-icon">
                <a href="#"><img src="../../assets/img/premium-recipes.png" alt="drink"></a>
                <div class="text">
                    <a href="#">appetisers</a>
                </div>
            </div>

            <div class="card-icon">
                <a href="#"><img src="../../assets/img/quick-easy-recipes.png" alt="drink"></a>
                <div class="text">
                    <a href="#">quick &amp; easy</a>
                </div>
            </div>

        </div>

      </div>
  </section>
</template>

<script>
export default {
    name: 'CulinaryCollection'

}
</script>

<style lang='scss' scoped>
@import '../../assets/style/partials/variables.scss';

.culinary{
    background-color: $mainBgColor;

    &__text{
        text-align: center;
        padding-top: 80px;

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
    
    .list-icon{
        padding: 30px 0;
        display: flex;
        flex-wrap: wrap;
        justify-content: space-between;

        .card-icon{
            width: calc(100% / 4 - 40px);
            margin: 15px 20px;
            padding: 10px;
            height: 200px;
            background-color: #fff;
            display: flex;
            flex-direction: column;
            justify-content: center;
            align-items: center;

            a{
                text-decoration: none;
                text-transform: uppercase;
                color: inherit;
                
            }
        }
    }
}

</style>