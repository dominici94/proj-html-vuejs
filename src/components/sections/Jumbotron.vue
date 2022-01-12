<template>
  <section class="jumbotron">
      <div class="small-container">
          <div class="subtitle">
              <div class="title">
                  today's pick
              </div>
              <a href="#">Food Corner: Top Japanese Restaurants for Sushi</a>
              <span>March 25, 2019</span>
          </div>
      </div>
  </section>
</template>

<script>
export default {
    name : 'Jumbotron'
}
</script>

<style lang='scss' scoped>
@import '../../assets/style/partials/variables.scss';

.jumbotron{
    height: 70vh;
    background-image: url(../../assets/img/single-post-img3.jpg);
    background-position: center;
    background-size: cover;

    .small-container{
        text-align: center;
        padding-top: 200px;

        .subtitle{
            background-color: #fff;
            font-family: 'Orelega One', cursive;
            border-radius: 10px;
            padding: 0 40px 50px;

            a{
                font-size: 40px;
                text-decoration: none;
                color: inherit;
            }

            span{
                font-size: 20px;
                padding: 20px 0 0;
                display: block;
            }
            

            .title{
                font-family: 'Roboto', sans-serif;
                width: 25%;
                margin: 0 auto;
                transform: translateY(-50%);
                background-color: $btnColor;
                color: white;
                text-transform: uppercase;
                font-weight: bold;
                padding: 10px 20px;
                border-radius: 10px;
                box-shadow: 0px 0px 10px 5px rgba(0,0,0,0.15);
                

            }
        }
    }
}
</style>