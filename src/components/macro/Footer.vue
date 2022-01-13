<template>
  <footer>
      <div class="top-footer">
        <div class="container">

          <div class="col social">
            <img src="../../assets/img/avada-food-logo-mob.png" alt="avada logo">
            <ul>
              <li><a href="#"><i class="fab fa-facebook-f"></i></a></li>
              <li><a href="#"><i class="fab fa-instagram"></i></a></li>
              <li><a href="#"><i class="fab fa-twitter"></i></a></li>
              <li><a href="#"><i class="fab fa-youtube"></i></a></li>
            </ul>
          </div>

          <div class="col list">
            <ul>
              <li><a href="#">Recipes</a></li>
              <li><a href="#">Places</a></li>
              <li><a href="#">Blog</a></li>
              <li><a href="#">About</a></li>
              <li><a href="#">Contact</a></li>
            </ul>
          </div>

          <div class="col contact">
            <div class="title">contact</div>
            <h4 id="address"><span><i class="fas fa-map-marker-alt"></i></span> 775 New York Ave, Brooklyn, Kings, New York 11203</h4>
            <h4 id="tel"><span><i class="fas fa-phone"></i></span>+0100-505-0000</h4>
            <h4 id="mail"><span><i class="fas fa-envelope"></i></span>info@your-domain.com</h4>
          </div>

          <div class="col download">
            <div class="title">get our app!</div>
            <a href="#"><img src="../../assets/img/download-android.png" alt="android"></a>
            <a href="#"><img src="../../assets/img/download-app-store.png" alt="apple"></a>
          </div>

        </div>
      </div>

      <div class="bottom-footer">
        <div class="rights"><i class="far fa-copyright"></i>Copyright 2012 - 2020 | Avada Theme by ThemeFusion | All Right Reserved | Powered by WordPress</div>
        <a href="#"><i class="fas fa-chevron-up"></i></a>
      </div>
  </footer>
</template>

<script>
export default {
    name: 'Footer'
}
</script>

<style lang="scss" scoped>
@import '../../assets/style/partials/variables.scss';

.top-footer{
  padding: 30px 0;
}

.container{
  display: flex;

  .col{
    width: calc(100% / 4);
    border-right: 1px dashed $contactColor;
    padding: 0 20px;

    img{
      width: 100%;
    }

  }

  .social{

    ul{
      list-style: none;
      display: flex;
      padding: 20px 0;

      li{
        margin-right: 20px;
      }

      a{
        text-decoration: none;
        color: $contactColor;
      }
    }
  }

  .list ul{
    padding: 20px 0;
    list-style: none;

    a{
      text-decoration: none;
      color: inherit;
      padding-bottom: 10px;
      display: block;
    }
  }

  .title{
    text-transform: uppercase;
    color: $btnColor;
    padding-bottom: 10px;
    font-weight: bold;
  }

  .contact{
    color: $contactColor;

    h4{
      font-size: 13px;
      padding: 10px 30px;
      position: relative;


      span{
        position: absolute;
        top: 10px;
        left: 5px;
      }
    }

  }

  .download{
    border: none;

    img{
      padding: 10px 0;
    }
  }
}

.bottom-footer{
  position: relative;
  background-color: $mainBgColor;
  border-top: 2px solid $secondBtnColor;
  text-align: center;
  padding: 20px;
  
  .rights{
    color: $contactColor;
    font-size: 12px;
  }

  a{
    position: absolute;
    top: 10px;
    left: 20px;
    padding: 10px 12px;
    border-radius: 50%;
    color: #fff;
    background-color: $secondTextColor;
  }
}

</style>