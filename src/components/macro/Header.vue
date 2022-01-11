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

.top-header{
  display: flex;
  justify-content: space-between;

  ul{
    list-style: none;
    display: flex;

    a{
      text-decoration: none;
      color: $contactColor;

      span{
        color: white;
        background-color: $btnColor;
        padding: 5px;
        border-radius: 5px;
      }
    }
  }
}


</style>