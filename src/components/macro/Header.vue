<template>
  <header>
      <div class="container">

          <div class="top-header">
            <div class="info">

              <ul>
                <li><a href="#">Download App <span>ios</span></a></li>
                <li><a href="#">Advertise with us</a></li>
              </ul>
            </div>

            <ul class="contact">
              <li><a href="#"><i class="fab fa-facebook-f"></i></a></li>
              <li><a href="#"><i class="fab fa-instagram"></i></a></li>
              <li><a href="#"><i class="fab fa-twitter"></i></a></li>
              <li><a href="#"><i class="fab fa-youtube"></i></a></li>
            </ul>
          </div>

          <div class="logo">
            <img src="../../assets/img/avada-food-logo.png" alt="logo avada food">
          </div>

          <nav>
            <ul>
              <li><a href="#" class="active">Home</a></li>
              <li><a href="#">Recipes</a></li>
              <li><a href="#">Places</a></li>
              <li><a href="#">Blog</a></li>
              <li><a href="#">About</a></li>
              <li><a href="#">Contact</a></li>
              <li><a href="#"><i class="fas fa-search"></i></a></li>
            </ul>
          </nav>

      </div>

      <div class="fixed-section">

        <a href="#" class="fixed-btn"><i class="fas fa-folder-open"></i>Demos</a>

        <a href="#" class="fixed-btn"><span><sup>$</sup>39</span>On Sale</a>

      </div>
  </header>
</template>

<script>
export default {
    name: 'Header'
}
</script>

<style lang='scss' scoped>
@import '../../assets/style/partials/variables.scss';

.container{
  padding: 20px;
}

.top-header{
  display: flex;
  justify-content: space-between;

  ul{
    list-style: none;
    display: flex;

    li{
      margin-left: 20px;
    }

    a{
      text-decoration: none;
      color: $contactColor;

      span{
        color: white;
        background-color: $btnColor;
        padding: 2px 5px;
        border-radius: 5px;
      }
    }
  }
}

.logo{
  text-align: center;
  padding: 20px;
}

nav{
  ul{
    list-style: none;
    display: flex;
    justify-content: space-around;
    width: 50%;
    margin: 0 auto;

    a{
      color: inherit;
      text-decoration: none;
      font-weight: bold;
    }

    a:hover,
    .active{
      border-bottom: 3px solid $btnColor;
      color: $btnColor;
      display: inline-block;
      height: 30px;
    }

  }
}

.fixed-section{
  position: fixed;
  top: 150px;
  right: 20px;

  .fixed-btn{
    background-color: #fff;
    color: inherit;
    text-decoration: none;
    font-size: 30px;
    display: flex;
    flex-direction: column;
    align-items: center;
    box-shadow: 0px -5px 20px 5px rgba(0,0,0,0.3);
    margin: 10px 0;
    padding: 10px;
    border-radius: 5px;
    font-weight: bold;


    span{
      color: $priceColor;
      font-size: 25px;
      font-weight: bold;
    }
  }
}


</style>