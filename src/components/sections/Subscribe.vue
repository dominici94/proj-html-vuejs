<template>
  <section class="subscribe">
      <h2>Subscribe <span>&</span> Receive A Free eBook</h2>
      <p>Lorem, ipsum dolor sit amet consectetur adipisicing elit. Repellat, odit earum? Mollitia pariatur repellendus veritatis, facilis libero modi dignissimos et exercitationem, eaque dolore aspernatur! Tempore praesentium repudiandae quisquam eos maxime.</p>
      <input type="email" placeholder="insert your email...*">
      <a href="#">subscribe</a>
      <h5>Cras porttitor pellentesque sem eu pretium</h5>
  </section>
</template>

<script>
export default {
    name: 'Subscribe'

}
</script>

<style lang="scss" scoped>
@import '../../assets/style/partials/variables.scss';

.subscribe{
    background-image: url(../../assets/img/subscribe-sec-bg.png);
    background-position: center;
    background-size: cover;
    text-align: center;
    padding: 100px 0;

    h2{
        font-family: 'Orelega One', cursive;
        font-size: 30px;
        
        span{
            color: $btnColor;
        }
    }

    p{
        width: 50%;
        margin: 0 auto;
        padding: 30px 0;
    }

    input{
        padding: 10px;
        border: 1px solid $contactColor;
        color: $contactColor;
        border-radius: 5px;
        margin-right: 20px;
        width: 20%;
    }
    
    a{
        text-decoration: none;
        text-transform: uppercase;
        color: white;
        background-color: $btnColor;
        padding: 10px 40px;
        border-radius: 3px;
    }

    h5{
        padding: 20px 0;
        color: $contactColor;
    }

}

</style>